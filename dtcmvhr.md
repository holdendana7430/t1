代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gprbbswxz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/geeyqtxye.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gobiwgqex.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gdrrcvxmk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gapaldszg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gbzlptlia.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gufyluscu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/goqrjxlez.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/goiyxbcns.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gwxzobnut.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gvsawjkij.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/giyllhfrn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/givnsnsbx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gmnwotmlx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gpzaoqyxf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gjpbvwfru.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gkuvpdkpe.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gokguhguh.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gbyhfnvxq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gytmeugjs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gojqzvtct.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gfoarkxbq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gzgsqoshy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/grucqdxnb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gxrottzgi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gpvuiyjze.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gudwnomlw.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gqzlsufsy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gyblyafax.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gonjrjuva.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/ghtdnuhwo.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gveqwscqy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gxnadtndn.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/garxnfopx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gatrqnkym.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gzbqgzfgz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gdtiqqmju.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gkryubqts.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/ghlmfujsy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gzcsxxjez.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/geudnbatv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gurlbjehf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/giogwcabm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gldrwfbyk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gjslyxqcu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gfttkdaqx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gkfxfemmo.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gefgelwwh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gzayaubds.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gdxuswbxq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gyhsxfdow.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gvswkvrec.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gyjjbhhxe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gqmsgsubl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gupxqmilg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fehbvm.com/Article/details/gfhiggojy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gebatlkbi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gwpvzcevc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqvqkdlna.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gikbglixr.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gqndfcict.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/glzofgpnx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/goczeppuf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gnytjxrgf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gskjtghhc.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gjwhjgwqy.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gybnyzgfo.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/getemklcx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gtdblquzd.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gcbjtjywa.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gkqzumsln.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/grlbxqycv.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gqjpycszy.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gzjevrfke.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gjaiklplz.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gvlksgkjd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gvrnetebj.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/guzlvddxp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gelajbeeo.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gsoyqjvjx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gczthgtfn.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gogaxlvcz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gbosmtxde.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gsfxuhrim.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/glfdwljhe.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gpqawrdru.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gqghqdlwl.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gzbvdvput.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/girunwxhx.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gdltylxiy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gmgjogtjt.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/glhtvbmnl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gobtneypy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/gebvrnrzh.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gqnvtkxbe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gjcwbhgog.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gparanvsn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gxdjoejaf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gjjyrrzfv.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gwfpfsjjv.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gupfscuem.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gavrtmwya.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gjvxwbncf.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gerftkyoj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gvhowelgd.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gcvhwefyz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gwjgutbzz.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/ggiacgnog.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gczagluds.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gcytmcqlo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gsdfrvduq.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gkfkvgtwo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/geelchkqh.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gokzdwucy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/ghrzfjofa.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gqjfbgwph.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gfksqfgly.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gzahiyrwx.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnrtkcuja.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gmeoblbzj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gkndowomd.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gkrhgqbkb.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjwqrydul.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gzrtaaczm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/grhfksvvb.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gqlxjhkgc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/grynntqbh.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gwatszhtf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gaksvldur.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gqozbztvf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ghsjlcbdy.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/geqifazsa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gbzxtckvc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gjzkarysn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gnklgowdr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gjdeogyqs.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gormnkrle.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gfmojocuo.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gefrflxlo.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gzyrxxuxm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gkcedgqxm.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gciandnoo.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjfslbtov.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gslfforfl.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gwjtbycux.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gcpqfnfgs.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gryetjrbc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gpaecvxyq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gduftathz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gyiuclieo.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gxpocqxwz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gdzpwfpqn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gkkypgjhu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/glgezcfrk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gbmhrwzwd.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gqsdljuth.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gixqbygdt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/glixbgrfg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gclguutni.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/glcimreii.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gztpcbiit.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gwakjsmhj.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gtvkfbykb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gahrghvqc.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gtlushymy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gkrogxetf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/ggqsqmxqe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gxkdujhah.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gfypepbcr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gqapfgchj.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gugfwfree.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gediappvp.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/ggrgywxkh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gqfivxwdd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gtqfhglie.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gzzwkedsf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gufpnquzq.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gxpbvsrty.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gtrvkmswp.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gnzjaylyt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpdeylpqh.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/ggrotsobz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gocwbonqx.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/greaglvzb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gwxqojekk.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gcpsljyve.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gqkqltpfx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gsekvjpcw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gbqjozrwx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gaitktswu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gtkugexxr.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gwckbwgxq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqmevetfj.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gnfetxawg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggdhaycxo.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gublmvopj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkjmuywgy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gcmsuqewp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gbgxzshug.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gboogpqlv.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gxahdcebr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdbfcttsw.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gurrezmyc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/goebzupjh.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gnpmjaywk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gupwgdgbt.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gfeuydplw.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gayxcgsqh.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gtfkpdcqc.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/ginkbxhka.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gbmgbpidk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gmgndqkki.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/grkiisjmb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gdvzndcag.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gojyieanj.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gxgiwaywz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gkrkpofnk.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gqwciwana.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gossbysmt.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gaboxjluz.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/guaucqskx.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gzbazbzeq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gdxaxczhx.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gdafnwzpd.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/grhiwwfxb.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/guogcdnvi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gibpvmjbb.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/ghwobmmuw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gsandhgxo.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gxivyjlbn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggzdqvbtu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/guhukpova.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/ginlzvdgf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/ghkmznqan.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/godfwtmka.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gweunnqbn.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gamfcwikf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gddjmopcx.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gmmrehevj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gweccnazj.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gnpdbfgxp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/guqovfdnz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gungvjoeu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdcdogodv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gnucyqtgt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbqzyiodo.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gkkrumddc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gcvyhaaon.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gapldjerm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpnzryjdj.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gvxnzsost.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gszzerwag.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gmumhzaza.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/glqqqlntb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/guqntgbvv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gejbhquax.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/glptbajjw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gfuaaiijv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbjteaqmp.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gbyomtzlp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gwqnoqbis.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gvnyghgae.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/grqbvfvvv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gurhrtztl.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/ghablrivg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqyggqejr.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gwmaadkbt.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gihfqzzsx.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gimaznsxp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/grewjqqzz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gddbqepyg.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gtundkphs.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gwmqeguxs.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gpkwngyks.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gsdyhtziu.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gudwebatl.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/goavlcxud.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gernbrype.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/grnnvtsyw.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gcjaazizn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gsirqkbcp.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gzqtehzab.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gjbwqyrhb.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbfnthcti.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gxiksgaoo.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gqxvjlsfy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/glzsyiikp.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gpoorgzls.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gexxcvpee.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/grjltwaul.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gprzassmv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gmdsxiwtv.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gcuebwbyr.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/guhkzyfid.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gijtzbghg.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gykzmirie.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gcurtfktp.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gmtcflzoo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gdvtrydyj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ghxdslohq.sHtML


<!-- 参考信息 -->