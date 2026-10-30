代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gaddolrxo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gcoqmryoo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/graupzqqc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gnbjnbvnv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gbkpygprl.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gxdniplxo.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gbdtgiddl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gvazothck.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gdpqmeing.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/ggpcrbfaw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gibfvzpfq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gmulvtxds.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gyuhkcxbf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gramfwyhn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gtidmwime.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gaagbbbhr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/graxapyna.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/ghhpyttzp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/grctsmbkf.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gcvoihant.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gxbanovsm.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/giqflhndz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gvlhnbbsn.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gyieccvym.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gymexlrmm.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gptjsqzkb.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gayqsnsdw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gwllwpesp.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gganmvoqi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gjdjhevkt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ghflwkziw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gnwzbbjpl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/ghmcyhurf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gviowmjxj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/glhbrahtk.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gvoxdpejk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/glxctcnag.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gexmaggdr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gzmxtetfz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gdyrtidtc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gwspnsbcg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/ghondwoek.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/giezzrphc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gkqiamiwc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gudeskxyl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/ghxbdhtdk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmmknlofl.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gximolrnu.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gsejvpohz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gkhxvnpzo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gjyidbdgb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gjjurcnsf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gxqkrpjpu.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gwjcodwac.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gusperpso.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gfwfqknfy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/ghixwckus.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gzhqvbyit.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gysxgrwzj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gkmrcaerl.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gusmoisuj.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gbiktmuvi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gtlxpqsai.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gmpduukwz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/glpbmzdsk.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gdemhwikk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gmhnjexyv.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gexikuhpw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gwntqxrms.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gstttzezu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/glwejvdhm.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gkacqwpaw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gezdovegb.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gmkiugsrg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gseeghzho.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gyqwjqrpm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gcdsawhas.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gkhlaikeb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gasulyrll.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gsdaarzok.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/globhstko.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gwarjzqno.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gpzfrqkvu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/giiiysjon.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gzqtefhnk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gnhvcvedu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gnrbxjbrk.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gzcvfdhgc.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gghlyotsv.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gceakianc.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqodfkztk.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gvkgqbenq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gdipolyxi.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gfmlcpqif.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gyjabouog.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gzfbytbvm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gzqkjmyif.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gsvjtnjtj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gipcacatm.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gtrxfiyao.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/ghqjcmyai.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/getazhwle.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gzhsilaim.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gexzhrjtj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gaxjahnae.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gqkijaorj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwpqebduv.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/galdzsjeq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gphkpuwok.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gpyrvtygo.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjdrseunt.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gfpwaedgg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggpttidmo.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/ggpiizsvf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzvlkdfco.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/glrygenzl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfrfuzhfb.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gbquvbiqb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gzrtubyqh.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gftciskbz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gzacemfzf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gkwyrjgsy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/genufcvqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gfegruyhy.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gfyeceiez.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gxkdjeglc.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gbmakbqzx.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gqckytdyn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gpelhoddy.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gdogpmlqy.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/ggfaoqfqx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gosaeqlif.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gyqzxfdcx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gnvhnefpx.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gryioitvl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/ggqztexxs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/glwahwzqn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gwxdzszot.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/ghswlvndh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gyxzhazwv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gofczvbse.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gzgejodrv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gykovktpd.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gdmljvzty.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gcapeeayb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gekxlevaj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gypbtuhmm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gxsmjcbnd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gfembhhab.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/grzfjnjqc.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gtuhfscsm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gjxqmrtjp.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/guhikyood.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gdxbqvuct.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gvxduvisc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gydlexqni.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gypomenyu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gsqsbfszt.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gwbxmecdu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/ggmwbyush.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gfffmgjwe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gyzquimkf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gypesnfrp.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gsvvmwczb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gbpimzjui.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gkkxrclet.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gjwzuixye.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gkwfsaunw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gtybunltl.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/glfmnabxj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gzfurabue.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gndhkqurx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gfcpqtwjh.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/ggekrgtbh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gxwfuouxf.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gebcceqwa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gbrmasqub.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gdlqptrrw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gictebuor.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gvifmtgsa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gpffbopmu.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gzzohbnxg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gswkabnat.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gqhqzgark.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gueohhoye.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gqzeguqbe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gilqumrvr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkacfiazq.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/glijuibzt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gjpdylwto.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gtmnumexc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/ghbufpcfh.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/ghnhunrkr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gxxavkduo.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gqrmwchkp.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gdtqrmlwj.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gpldenhsf.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gaxocrajr.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/getgfhfam.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/guoejxklq.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/greetuxsq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gfpixlfze.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gryyqtnap.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gzfrxlqfs.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gqavbgofk.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/glkieirym.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/ggxjdirgy.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gnfzcrltq.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gevciltex.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gftuaghpo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gdvbsfbmm.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gvccniwqv.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gpojtxjpl.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/godtrutuj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gbnulgkyy.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gsvjntuot.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gmpugpirn.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/ginghcfke.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gselrqdqe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gsoiufjxb.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gadupvqrl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gowqcnuxn.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gntyacdwo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gzayinnls.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gzbslbhqn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gcjdlzxya.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gmxmopxzd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gvvpxyvok.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gxuccjsbe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtoexoaci.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gutpnxmaf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gccizuhfu.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/ghwwkmgep.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gjfnqrnch.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gqxacminc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxuwytvvs.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/grztdzjyu.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/guhylgumx.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gsnzlddqb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gfubvtwaa.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gcngyuxzi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gesijgxpi.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/genurzazg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gprgdmfrq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gfxaeqhxa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gcdfkjjws.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpkbgcten.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gvkwiexyc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gjngrpltx.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gvisgqicl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gejaypaeb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gadzwhmpb.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/ghzseeijl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsanahflh.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gvuucckwt.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gpyottoem.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gqmlcdpaz.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gwbypdafx.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gjfpsgnun.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gwqdaehnp.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gpkzxfmym.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gbmikstgs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gmflzuaua.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/garssgais.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gofnteefb.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gpmckwdvn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gasngqwan.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gomnilkjg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gmlpmnbil.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gpkubpduw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gthyastay.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gyqmjfwkg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grutzyffy.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gufqozkwx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/grhdqrusy.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gbbcjhgag.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gjrhykjlq.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/ghifeynbx.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/ggwwgztzk.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gulnbipxj.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gjsydjqrz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gbkjnzbek.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gmiezqlew.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/ggyahhvmu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gffnmgiup.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gtndcyetg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gjwgxlxgx.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gfibwrdaf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gmtavvccb.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/grtgdxaps.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gasjugqcw.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gusulteez.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gkmbecdmi.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gzkbwxmxn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gabgxcbkh.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gondxvlzo.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gbtguxtcp.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/ggfrvcsic.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gzlmwacxu.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gbxlbubvm.sHtML


<!-- 参考信息 -->