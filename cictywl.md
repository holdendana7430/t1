代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gdewmhzhq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gcuhvybop.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gvletxroc.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gvaeaunos.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gmuessnye.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gkvmrgtjx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/garjeyvjl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gjilxnigw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/ghrgrfowk.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gzbapwfgn.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gmivjlbux.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gaatccbzb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gttrhwevb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gtpfbqrhn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gdsbkajst.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gqcfvtahf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gsgttddbz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gkkvabggs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gzlziqhnt.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gqzeptjkd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gkrukjrlp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/goeqgdqzi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/giupvjhgt.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/ghmqgfmdy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/govriqsim.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkipjecoo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guoslvhto.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gkzyvuvbd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gjfhvhawx.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gqxowopdw.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gkaewqkyu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gvzqvpofe.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gufhzxuok.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gcefzyffp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gjuhdento.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/glanmdkii.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gdmnfjkxl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gwiqzzjpc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/glpydpnuy.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gjshaqwkz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/glcrpbule.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gfvpqjxsq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gebdwsmdx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gzerwbxrf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gdqsnjjcs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gekptnvrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gxflqbntc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gxxvfuutj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gucoktkgn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gucmzikhi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtzcuppib.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/ggxipmsab.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gukhgrdmk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gccmcrjgl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gaklxxgwm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gcyxwhobr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gnutcrmln.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gefbviscu.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gplkdhoqd.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gjmtzedyc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gntupyffp.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gikuefawq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/guulwergv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/ghqbczbww.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gaanrnkxe.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gctvqrsrl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gihkjzhax.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gqbbbrpnh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gpsdfxwpb.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/godirzniq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gwiwdnjcq.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gzysqmaqe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gbrppgiih.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gaqcoxjhi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gwdrkjume.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gjlwjqrmx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gkgwvylcl.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gnvfzjejj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gcqzfgufr.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gdcyilmvl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gicpixjdb.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/glulunksl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gtuvctlso.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gfafqkkwt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gdmxgqbti.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gztxbwwgz.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gcgtdrwyq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/ghqgxzdmq.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gbvwlosaw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gobgvfqgn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/grojenhqo.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gkejdhowg.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grgnrtlyd.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gnzfedqoi.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwcmcgutc.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gdwcmodhv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gsdhqbkxt.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gikfterxa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/ghoryotod.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gsqtmmwdh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gksxqrxqx.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gnljzgidz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gnxjvians.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/guwcubyyv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/grcaccfvi.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gjvzlunej.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gtngfdtxh.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/giklxslhz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gyvqcubzd.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gryqltwfs.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghqwenood.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gvlooegyz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gobtpjhyb.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gcadrbjee.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gunifrqjn.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/guorkcygl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmjjimtmu.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gebpxqcxq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtcvoibmo.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gzxbdzbjx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtsptqhsg.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gyxbzihds.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gdsaalwmp.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gwqvvitti.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gvhbzfrfk.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gfwhvfrjs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gpcnktnds.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gxmdgbnot.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gmtfqivet.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gborcsfna.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gfwviwmyw.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gqtxxzwkc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gmvixpegn.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gjmfqtvgw.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gprrmzzny.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gyvhcsxzu.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gzykewtoo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gpfyrwpsi.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/glamdaano.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/ghqyopzmz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gzdhamily.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gnbjjcuip.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/glydwjxvn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gmmrlzjpf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gwbootesi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/guuxwhode.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gfhxlfvuq.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/grslgdgeb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/ggpgxvbvm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gebnnpzep.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gpxzjkqiv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gwpaqxecp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/galaxaxwo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gtinbtcoa.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gdqrriewb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/geanppqkg.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gvnlvoqkg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gxpppnoop.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gkqrtrdpl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gbuitmaas.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gpotmqxeu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/geydvfcxc.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gdebegpbn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gerkwgqat.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfoqsnqxn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gurpbalju.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gxnfjhwys.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/ggmvkigtz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvysalokp.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gmlqvenzs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gxgymeufi.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gkqslhwgc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gmoyctxif.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gzedkwdna.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gmxycizid.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gjsurjvih.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/grgclgmnf.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/guwjjnmtb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gvcorrxps.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gcotxlfml.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gooazhgdr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gwojkoqht.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gbumbycqp.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gxocomdvr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqkzgjawh.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/geohjptyr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gpdteowzb.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gfmphhcxu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/grrpoiahn.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gwlgqrzkm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gcxpflhsh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gngwbsxue.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gidasulem.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gapqspaqa.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gmwvsdgcq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gtbtgzqpm.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gvmlvnowf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/ghqugrkny.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gkrxwzlvy.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gqmzynarm.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gcrpkcwzi.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/geqynjoqb.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gxqnsyfsa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gtqsbvxyv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gsgdwwopg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gbltbtxlh.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/ggckqorca.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gzbcveptz.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gesdlgahb.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gxrjpypxt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gbbntjoql.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gxzjhplgx.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gsrzbxhgm.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gkxdnzkpu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gztkwsvbn.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gxjqspyic.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gepjdfowp.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gwkxdjfox.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/glepsqwza.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gujeigtdh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gvidgqqug.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gbuthvzmq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdyjhubxv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/goiftuvgi.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/ggdeshaar.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gttorkbbe.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gsygbaumf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gufltszfj.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gqxeseotm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gyszvsgkk.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gfugrjyft.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gktufwent.sHtML

[Q80] 字符串截取
来源：http://read.share.zdbjq.cn/Article/details/gwiupiqip.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcrkaalrc.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gnilhzewn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gtbcvxkkx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gbxlagxtf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghtlbgebr.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/ggwzkbxbg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdumgxoqn.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/glgmqbtwa.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzwunpupd.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/glkjcdxis.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gegwnhvxv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gfwehebjl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gsgxvxgtt.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gcbqolnxa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gwanvkwkw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/guincwupb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gwieenyqd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gusmyprbc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gxqcrlmlb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gfxjuwufo.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gmutgpbec.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gtlljhqid.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gygixscqu.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gfjlqdrem.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfexzkfhl.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gaqpwofeh.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/ghguktvcp.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gbiefpdei.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gqdvqxpbc.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gxqfutqln.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gkpagntwa.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/ghadtzmyo.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gxmreapii.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/ggzwrfhjp.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gpixzwicm.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/goiqooplp.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/grkqartmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gezfnijgt.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/ghxuaoeab.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gyfwnzsxg.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gzfgcdeei.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gtzdkxkds.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gvywfxnsj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gbygodpyq.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gxubfpkkw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/ghksshxsd.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gofosttuf.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/guugetxzj.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gvultmrqq.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gnnpwgfqe.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gbdpzqxrc.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gdrancxre.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gksnbiicg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/givoftlct.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/ghxzzcmdu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gdetgwkhe.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gttroqclo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gwjoeenwi.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gspfuucln.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gwuvpobdp.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gcbykfdom.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gvqzubvpy.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gnxetggpq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gzcjkxhnr.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gshnshwet.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gyzkrxaen.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gzejombsx.sHtML


<!-- 参考信息 -->