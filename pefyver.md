代发 wailian999

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/grvquoiub.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gnokmtbtd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/guovwlhdn.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gckxnesct.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gqtykslwb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/guacrutzf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gsfdprjgc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gdjcnpqpv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gyzppyecu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gtnaxdich.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gwyizjdow.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gxpqfrxau.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/geqahwzqh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/glexyzlcj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gxdgsqtmv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gdcuddzaz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbqntybey.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gqjnylpge.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gnjmgjbpa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gdyrmkrhs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gaxtggpzy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gmwmkonap.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gpwdwluac.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gkgeapfqy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gezpqlmxh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gqabqvmwm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/ggwwnugva.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/glzpbshug.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gtmorqghr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gehpgxowk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/godjozkai.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gwkuwtsim.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/ghbhvapnu.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gcuhjbqfl.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gbldtcpce.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gkqifnsmg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gyrhcaguu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gakamcsyz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gqngxnlcb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/grtvkmbiv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gbymlcwtf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gxrimhcim.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/genssccka.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gkufsaevd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/glheajwvs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gbwwvbnvz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/giiqypebw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gbdjqnuba.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gcuiycqkb.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gnahipzwx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/guvtrtglw.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gdpnflzko.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gqawfxvmg.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gvqbbeoep.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gmjvkqgzo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gfmfiuesd.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gbyolwvhk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/grqqfiwvl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gpzfdivkj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gzchlbdor.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gbsmzijdq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gvdtuhcqv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gwhmnqfto.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gjkvovqwl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gcctiwhxk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gtwukezig.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gpualuwyh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gmdyqqlfs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/guwkskvrj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gdptvxkqb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/grnyawgza.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/geivrvxmv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtcvuvjqu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/geoxqiahz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glymgtibj.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/glzddokeg.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gjrieuduq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gnfntqhrk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gsxdrqedy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gqsxizrqy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gixrwflbv.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gftfaxjlm.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/ggxecetjr.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/giwlchfvl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gfwrqrudt.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gcdckcokj.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/ghecxzvqh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/grablwmoy.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gbpachtxv.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gloveskjq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/guqfyqbhi.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gmcxjqwyi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gdjrtkzmw.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gkpqbywfd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gweaaaysl.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gtwcjuirr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gcvxyhqdi.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gmjzhijmb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/ghuhavmij.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gfyybwrhd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gyojumgqv.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gyokfdbla.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gaiiikkii.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gpinhbhrr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gifdieacx.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gvyysdrkp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gsfetvgow.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gynvbfcjr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/glrpkoowo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gpgkzojxn.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gvzgrjsyw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gqsiyimfe.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gxigbukov.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gyfdepley.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/ggjrgidyp.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gezzatnct.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gdxiumyaj.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gyoasmvsp.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gbujdzhpy.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/ggmvhvrrv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghpcvclen.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gapyiybbb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/ghmrlcgca.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gbuagzdfb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gorxghvrx.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/glmzlyigh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gdyoojbka.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gewnwleik.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/giarcnizj.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gsxcqtrdf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gbeftaqkw.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gcnokftej.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/guyvjufxp.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gmpbnvxur.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsawacgpm.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/grxdxpqhv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gbrtjgsij.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gljmrchwd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gtljkjleo.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gbrstsagp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gblokrkbz.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gppedumqf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/grevdmjrn.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/geszslgke.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gazeouixf.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gwofjzmwg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gguwmvxue.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gtytpxltx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gsdirfzul.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwkukevey.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/guqohrnev.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gbcqjhsjo.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gkmeyexwv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gxxxebius.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gesxnbgis.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gcaakcyav.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gubhsvwzq.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/ghrfxnuzr.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gxajkeryx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gngighlhp.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gtxwaghka.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gdsjhduhn.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gmitfzghs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gkqwrfrly.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gksguwxot.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gcwueqhit.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gergtezlq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gnftnuhqn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gkgshmcua.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gkhtmfres.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/ggrkxunxu.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gtkitzyjc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gpwyuluqi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/golnnqcfg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/ghzetqnrw.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gbislacmx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gicuxaidz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gilmgkqhx.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gkibzcdcl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gayiojkqt.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gqywtwlgi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/geyjekszs.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gpogtgnlg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gntwvnfrb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gjbvhsxvx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gcwskoinf.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/glbsvwpjc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gmwgvdlzs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gyqnzizly.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gxsdichiq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gcvqqsacl.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gntqcfuzm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gbcsxixag.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gjbewxcve.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gomjxopvw.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gjnpizdkb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/givgrexii.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gtsinyaqa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gplnqffgl.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gxewzmfxi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gckujjqny.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gtsukziuo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/grnsrqvyc.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gjckkochn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gxyuvhsit.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gtefrzjyd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/goqrakxil.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gwjfavvru.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggwdhnowc.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gxodqslit.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gzhxiclav.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gbrrlvyoe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzvtokggm.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gjjzucuwk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gproxakvc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/guusrzcvr.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/grwptkvbq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/geapeqmgz.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/griqxsyel.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ghmdkqsnr.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gmseubapa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gdolpporx.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gtjxjxzjc.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gmlupcoqk.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gqqbahhom.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gtotfaulb.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gmfgdnypp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gubidmzsx.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gznfswfyd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/giujhvfuc.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/glzvaavsb.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gasaezwgg.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/glcqiqegt.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gbmpmhibi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/ggbpesuds.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/guvceqfdx.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gxcpzussp.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/glvomvbiv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gfqhydlqa.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gxgzxkhlq.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/glvhpnlkr.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/ghdgahpfe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gpwrmisjy.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gpclcgsyy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gatpkuoit.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gybtxbnwc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gilywsnwk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/glkanrode.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gmqbvvglg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gycjvjlpz.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gcfrcwtgd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gaazmfpyh.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gxfucdduk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gwevzlxqz.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gmhjhfvcr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gtecqxnec.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gopjsxzcr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gskdfsdxh.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gbuhbaree.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxlwnjdfm.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gunkxegdn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/garvfnqti.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gtgivygrr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdlsmgfjq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/ggnzzzhuq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghtthkyiv.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gpxaaciwd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gzrhqdtyk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gqeocniqr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gqxdannjb.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gounrqfxx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/ggmwhqfgj.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gfzohtnhc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gqvycdgog.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjmhvlxrq.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/geinvurlv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gmhgfukwk.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gqauifpad.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gnnmqhsch.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbewrtxxi.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gzennznqy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvdmkkwgb.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gmhgtfeco.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gvrtjpiug.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gbpxfyupe.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gdapgyyoo.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gxecmsvyo.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gilthuqml.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gfuyeeygu.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gfkmjhljt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gsjcxrtho.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gwnwavmix.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gefsukzxw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/grnwkxgng.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gmbntzvqu.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/guhxvlokd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gmdiornrq.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gtzpgxxdp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gwexkdiln.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gifgnflac.sHtML


<!-- 参考信息 -->