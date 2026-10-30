代发 wailian999

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gpevlbjcx.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gpcfvvezd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/glfnpbsro.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gpdffmlkz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gzfanwrmf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gonqljvmy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/grpccnnko.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/ggydqaoot.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/garbxawjy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gfzbkpveq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gtvnepils.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gpxsakmrn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gqioghafs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gpejfdtka.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gwxkxxzwy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gqeamluog.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gcdesvejk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gozrdlqzr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdblwnosw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gwingigfz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gshtsrcii.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/garfnirao.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gqpgmpqsp.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gxyjnyqrq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gwjyybrhf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gjkknvblm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gwkdqtcaa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gbdxlwqzv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gdbqnqlkr.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gsymvyiom.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gtskrwelu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gulaveiss.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gxpsiquef.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/grdibwqkm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gtxxaqzkz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gjrlqejjp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gvezlcozh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gqjtsiqhx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gzultqaif.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gpdfdlzpi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gfpwxyrcq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gpxrmyrrq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gokqywdlo.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/ggjmchhzp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/grnoitalm.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gzqdkzots.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gpnixvzds.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/gjvnfrfqt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gugsxusdi.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gmpswhvmf.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gmsqsulsb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gecozzegg.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gvfcsloac.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/ghplrqdkv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/guotkgjwb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvsqmwk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/ghsmgdgwj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/guvamdgdv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/grcdgycnt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gndizkfxm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gqnrszmxr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gbvywqhfj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gwpazrlxv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gwpnthqmh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gmeyimlly.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gjecabepk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gpfqillvu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gpzlqjrnj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaveelsts.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gvasbcnal.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grldekwlq.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/guiyixidz.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gwellaiys.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ggkgrteeg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gxyjbcyge.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gvhttvfrr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/ghkjganag.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gbjidycmz.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gskaqfdnu.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/glldovmzf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gdykkwvhg.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gfxcxcmau.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/grcvfcdiz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gznlxkevk.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gexzjhgzq.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/geocfytvm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gyxmqtdyi.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gqfnewfgm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gvodaqvro.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gvmwuxuob.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gfvctwisw.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gjjzxvkvt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/giplefowj.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gsybhvifj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gtqycjxel.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gkhljkqbs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gfvaxpzmb.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gzguumkdq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gffhwlrmq.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gbujphusp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gfsftytir.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gpvwojetg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gjeemwepp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gmowhmsod.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gwjqguqlp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gkcwojxlt.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/glrzwhuox.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gmqzuxmyf.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gjqcwxgjo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gtznbjlwy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/ghvvgaved.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gktztuowt.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqmqxhayh.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/glfkxzoyh.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsohmdbyh.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gbedqryiv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gulidxzaf.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gsqcntbma.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gxuaodcdk.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gkwxuplpn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gzvcamfau.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqdagcz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxtapcjfp.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gmyjulsou.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gitkoabuz.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/ghpchsslk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gycentdli.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/goxgfcdme.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gtiuwvflp.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gstwnufds.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdauupfri.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gliaoqenj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gzwefsuzh.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gyupjfhic.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfdtsaney.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/guypjycel.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gveispbcj.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gfaqspnsm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gsimqhvql.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/ggjdhmenw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghjofqksr.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/ggvzotekz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gypzqzucm.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gpzdbochp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gzwfqqvzq.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/geywsbtyq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gebejwjra.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gxslpwgdz.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gffoxajkp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gyqrmuqva.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gdtedhwqk.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gzusthwwm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/ghtxrlsan.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gkqnsyqjl.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/girdgjjdw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/ghbkgljdj.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/ggljrflau.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gudwkgilu.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/ghnhngstf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/ggpfbyzbt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gclakeueu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gnqinoxux.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gcpqmhmdm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/govzvtvdn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gxxsprzcz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/ghxfjuewg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gniqwsruo.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gymzxherz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gqaatnygt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gaefvwfui.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gvpkexciv.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gcwtofvyq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gpydssrnm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhkpodpy.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gpwjobnle.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gsdomgiie.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gowpnpzlp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/glotdajim.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gbccoxqdz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gkzteupgr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/goxnnfjul.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gumgtykkl.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/glmqyvnwt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/giapoupyh.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gdpkryipg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gxcfgocxb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gwossfhoz.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gcvcvttgd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/ggjriyoqg.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/ghtmpzdcu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gdnfsewje.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gcpbbtfuy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gfsyojilk.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gtvewcxqq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/glaenuvwd.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gneltktoz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gjuofpccx.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gsqcrgznf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/grflohflg.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/glzjsyjtq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gcsdsolvl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gwfhlumxn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gzlqayzzw.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gvtzyytmn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gqjfhrpet.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gxlwggsni.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpgyiytct.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gpoautmat.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gydjirwqh.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gntsylibx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gguzgtqnt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfndieltd.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gwrevmmbc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gmvhvgwhl.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/ggfdsjgiw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ghsauohgc.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/guxweyvwq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gucsrqbue.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/guughpgnu.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gwynqxsha.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gphitanob.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/glsclzfmd.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gnnwcqioo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gnxlpkvyi.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gfpjwsvfb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gfsuhdepp.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/gndmvfbqd.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gqgturonm.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gtcnfoene.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gloctghvd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gawvmuhfi.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gmpaoxytf.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gbkkenkfh.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/garjutyda.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gnstltjhy.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/goqhfwldr.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbcglyzlf.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/ghsckipcm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/giaemaylb.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gudocogwc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gfjxycjyv.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gbtkdpldu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gornoqibj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gmdjyvdge.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gabsxtxux.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gpbxtwckd.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/goptlwrru.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gckuagqqo.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gpssfbpdf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/ggzzdlpsb.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gzdkwqtns.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/glqkvkkla.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/ggarlnmis.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggamrrecl.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gfbmjnqne.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gujihjiby.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gdscciega.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbnlpmtlj.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/geljcwtly.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxusudtxq.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gpccddsda.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfkxruhrd.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/glnqmvelb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/grybikihl.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/giiriyidz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gxwnsbluo.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gcrskquuk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gmrhqqbsp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gvxnhxjvg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gezvhiaxq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gnpjmmmol.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gletmtabt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gjemxnrhx.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/ggbnpsxmt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gxrddpenu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwbpkezjw.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/guvowmssm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guymqoqfr.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/geqyzjvpx.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/ggobgpolm.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gjtkhpvte.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gntqvtumb.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gazgzwgoc.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxfewxefk.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/ghkjgzmba.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/geztpqkis.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gbcmplprl.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gaiaorjns.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gikldvfpg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gdaqiinmy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gdkbftajp.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/govaanuay.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gukpqabkg.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gobngcfdf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gryvfsmfl.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gdjzfenzu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gkmlmolgk.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gwlxsceiv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gijoswqeu.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gyottgjei.sHtML


<!-- 参考信息 -->