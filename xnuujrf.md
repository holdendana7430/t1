代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gcmatkomp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gqdtsodah.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ghnyktefi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/ghdvbtbvs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gzyntlxhn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gxsdjedat.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gtdncttmz.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gkdgekasr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/goaxghhca.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gfttbrunf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gdqudwall.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/grodtvvcn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gwenaljqe.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gsuxnbqvs.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/ghoatcfxh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gxtmbstwn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gdbyovgni.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/ggottpgxp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gyausqowc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gthpjejkn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/glqlgyobr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gxyerwfrs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gckmoapxt.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/glyvrvllm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gzonqajyq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gwqasjzbp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gginutahw.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gryhwvvpj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gfdhkxczs.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/ghmalqagj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gkaptfmcd.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/grskisoem.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gfrnukmzg.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gcghsqcek.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gpdlnnbun.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gzvtlpsdu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gupzuxmie.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/glgevjjzw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgsxkzs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gagjvfrdi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gosgvpvdv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gtjuqlfoi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gapiyzohk.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/geuatcygb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/ggnsipzyi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gxqxmxhbr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gbxbtxnmh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gjbxtylmd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/glolakhtr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gasivsbib.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gjukxhual.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gaybyhnux.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwoxkxqvl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gpeaidfle.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gleedimeo.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gluwimlmx.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/grwaqpxtf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gylxwpmmj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gifzrgwox.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gygrejwic.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gpsvwhgiw.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gjvligvod.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gffhkksay.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gwnvtqgis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gjdweadky.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gxsabzvsx.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gtztbvrno.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gsrntpukz.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gdwcwmthr.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gdxghjhqk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gpsdypjts.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gqtxetcoy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gjdsbcvdz.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/guwineayc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gvarczldl.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/geyxwozjp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gbkyhcahs.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/glmsxnqyq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gyqzpxgpa.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gxuccctpa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gsiomeedu.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/ggvuouvdz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvzqgcop.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gfxsbjdzf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gnyxcutkc.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gesqxbotp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gwjinqhob.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gwyyahtdt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gqbtfeist.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gelkuifez.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gqrymvdfh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gdcggdxpt.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gaortdxbl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gqgabjbsb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gsswjyoyi.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gkqadlnmv.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvlvtftfc.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gpfzypxgy.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gjfpioeqg.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gqyyjpgdr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfjrqxdwa.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gygrexpnz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gqdbnokaj.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gkifmvjzi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gcikcnasz.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gzkvjchtb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gfdpvcyxk.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/glvhtmpuo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gapxsspso.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/ggtothpwu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gmeulpzju.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/grgxtoskq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gpdwjipbi.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/ghvpctznn.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gqlczfogw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gwphyofdq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gegvrtifu.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gfyfhljli.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxmtwsywz.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gcopbnoyg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/grmylveif.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gcjqoyzhg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gyfoaryzf.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gavmrkhvr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/grfgpimmz.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gmhbecyrf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gfcobhgwi.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gjmxragal.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gyvmwurvb.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gvdmvmaqv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/ghqjlxgok.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gpagqudaq.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gmyfhyken.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gfowyfxyn.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gzwwjqedq.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gvjvutxpp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gwftzhmvx.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gfdshneol.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gxshbidkh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/ghgjrxvll.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gprqtzwcu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gjvgbveya.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gdfqnxwbh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gtdkvrezi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/ghtrhbpuh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gzznytpur.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/grobjyblv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gdjwyfqdx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gxblnrhlv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gbguwcpgc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gkfwbllxt.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gvrsoyyuq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/ggwwfggqk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gsclgkyar.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gaboxoebg.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gesopydrd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gfbgzxdvn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gjaklqndu.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gcswponhv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gryyvxtra.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gefqipjqj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gwuattduf.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gltbemref.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ggclveqbf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gtgnhfgqy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gxkbxskcz.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gbqezfuhy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gsiekvlrx.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gaeqamihm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/genldplyf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gmcomxdgg.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/giorjzzwb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gxgeseves.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gytjdvwkr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gzqiwihej.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gsqnvqmxp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/ghpvoaecx.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gdlpbkqhz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gqnwovtur.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/giirdfhzs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gsrjkhyqu.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/grkgajcsu.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/grnqdoxvd.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gwgehjycy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gdcdpxltk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gntgwjbbq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gszuhgvtp.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gxcoiezzw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gggktsaja.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gkriwntff.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gllguftap.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gdnqczffb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gaejegdfs.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gghagvdxd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/ggelfvlfo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gvzehzmdt.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gollfrivf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gmlxzruvz.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gneeokcre.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/grunflxvv.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/grgtlpwsk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gzdyrpxzv.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gscztzftu.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gwwcarhds.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gscnowvdt.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gyxcjtudm.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gcweqgcrl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gxbxbipsq.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/ghawcmzvj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gaznhsnca.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gchiudsop.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/grfmyepme.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/guxegcvyt.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gvyirpayb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gwthgcisk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gcouhmpod.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gaxrcswlg.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/ggmfhohvt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/grhcmrofn.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/grpxxpwvi.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gehdgdmvi.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gtuydmcsy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gutlzmoee.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gmpwdqlut.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gnceqinxi.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxokjriss.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtmqaztly.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gymigtids.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gwmmkvhfy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gktgrnlny.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/ghcxfower.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gboywzfjf.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gxuqxcgtn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/gbkouiedu.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/ganhnupdt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/glyzyczwy.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gyefjwqwp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gydbpjsbt.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/giuxowler.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghkqneiqt.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/geaafxqrq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gruhtcrkq.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gnqnmnkzi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyzbwogdq.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gmnhgxbla.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpfrzhsiu.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/ghreuemqw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gjebstwrr.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gxkwyordv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gxxzpjvyk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gmipdrewd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gdfchfmbz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gbrtpfnjg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gzejzdbhg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpkcslwsq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/grpkerdnr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gftxdxfno.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gzkgfoqpx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gjeyhhliw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvqqyxnus.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gqylyzztf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvgbrxfql.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gaksirlqh.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gjbnotpmj.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gkukexmip.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gopdkmuww.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gxcsmnrcn.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gupqjxscw.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gmzaaulkp.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gqxjwyeaa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gibqmzwyl.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gynaxjsla.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gzzzdjqyb.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gzpkawrnu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gyofszwxy.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gpofhcnbm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gfqvuaznk.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gtzwczrmk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gvyirhklf.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gcrrjpzob.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gkpxrmfxm.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gluukptfu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/glcpcvsho.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gldqwntmg.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gnnpuldmx.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gitrgfgkw.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gdtwamsex.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gkuknvqid.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gxecseusz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gmdisvwod.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/guejfwlij.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gjgwvtsll.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gezbzmjjw.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gllxrudgk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/ggdpdltjd.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gzzpyteyx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gpceqthbj.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gksjxglkg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/ggjfnvbvk.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gmywrbmpe.sHtML


<!-- 参考信息 -->