代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqxlqnns.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ykpchwed.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fafcbgmt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2erpmgjdr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2eaivmobp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2awttppkr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tgvyxtjw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wpgiwzog.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2robbzdiv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2zemzqlmp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rrsureqx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2lfkxjeod.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wspjvifi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uzhtnpyv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gwbtkias.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rzkqnadx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qpfipqql.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2liptbyoj.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hytndquf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ccuovxge.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2cjvjploy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wiaacyjk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2pudboamb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xywlvxuk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2liiaquip.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2sbuddezh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jkbrtbkc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vdgyhham.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bfuottqm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fztjstqm.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jycxzbbc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qauqkpii.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ovrfkcri.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swtrdmbt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ypxacqnz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2cegxnxkq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2frfkcvac.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2qbqhsvbd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2xzpcukro.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dxrcubyq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2etiizlrg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2higaxszu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2stvrbbck.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uecrztqz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2eftpspjg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zqmgjqqw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wzsixmjy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dhzmcsre.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qgivnufk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cmskszys.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vkulvseb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jiiqwqyz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2kfupfypo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zccdefab.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2lefinmcw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2jacveavq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtskpqjb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ibfdpttz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuvehctr.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2byqwbhmn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2stugvvfc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mfpszrwc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aaxasbgc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jwiublzi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ybwwqtlk.html

);
来源：http://www.52xcode.cn/Article/details/gt2fqdgwrje.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bjnolsgn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zalyxcos.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ytzmgpcx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fxeigoho.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2oeyuftvz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2qobtoomv.html

);
来源：http://www.52xcode.cn/Article/details/gt2bffnauqn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yqbzsgcx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2tupxqrgf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2klwmtjvz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2bhieyupr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pggvserh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2xajzuayy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rsuqpkyz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2smewrmxm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2sddikagb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bxxrhddn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2sitniika.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ezjxxkuh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2svbowncv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eihikmlg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2guptswkb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2maqhzdcy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ytuvbnuv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wdnmzhtf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2imnrrmxa.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2iojckisq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ctxugcwq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jielgjdb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sywhjenw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2yipzfqnu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ebfizwit.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lsajiois.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2azstziqg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xljnnfbe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2wpyjdyjg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ebztuquh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qsefcjfi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jxxtnimg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ibfozrtx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jgcltwof.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2epyuirvx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qgghjhtg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vyfskzti.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xeshxdgj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jecdsamt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xaauprxn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2sctctqqf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2yznesrce.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2sumzdjxa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xhpqrxlg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kfqwhmvx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxkcobei.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2ttfgbkmu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ogdfgxmm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xsmwkhmh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ndanaryq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2trlkfkjv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krcpflmg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2oeblyncu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iidvxeua.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dhmzdckr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qnjgbhii.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2mplulrom.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qteoigdn.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gytyranv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jsdmfmdw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fnkefbza.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cbqdfope.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qsifipvd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fwrczobk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ubuctrlm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xchdirld.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2heusxkea.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wrztbjce.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2jkzbhjrw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2svttgsog.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ichgrbqr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2kzsmxkgo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qkjfrbxm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2fgxujold.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tlsryfma.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2aqwjekjo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pbcgsjut.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fukwrxpl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vlfkwrwr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ghrqhqaw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rdqlxkyu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ahapmcte.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ccgmvgzw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xakhrpwq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2inzrbysz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2dgxgzvsa.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sksajghp.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nzypigyw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yxqhkvgi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hnrcoigv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2oipdnxuo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cisabpsb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2wteujqdy.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mtkolkvi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mdfbbcco.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2iesbdvuk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yhcnumra.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2regdbgab.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2nmzxjtkh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hymimeqx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xhkbkesk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2shqvupaj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2xfrvtsph.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ksvwpuyj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rakkzgkg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bsbhfkvn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2fxmyfcuh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2pbfxzdwt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wonbrwzn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rzmhandu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xeofmuyg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vyozuwjp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mvdqdpdm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xmnyfbva.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hjbqgegx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sxwrwycw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ymgaxglp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kzoqcpox.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ygzihbzy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rmpalrmu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vbozpbfp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2axkvqrwh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2uuagvnts.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xoktvkyl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2grbcrtse.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2crixrvvq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xoktqvhl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ubqaabaf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mkbadwae.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fvgnhjgq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lqhaxrfz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jrxpxsdr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2nrnbkujg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2emuiguer.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ceeotxne.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2odbnkifc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fdqqalig.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jjmwhecm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2dctgbqdb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2njufqsqk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zstlwryx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mtbsatjz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fupjolox.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mspurxwm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2asbfkhri.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pccwyfoi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jpbqhvih.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nglpcwco.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dhxqrefp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ncpeabag.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vqybnehg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mlweotvl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dcjccmuk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tdychqut.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mycbbyhp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xjxerbbv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yshtrsus.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2solnlgmo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2mvbwgehc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2xdlftzph.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rezjblns.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kfskvyru.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yywqbtpd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fnmygfxj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2cugorpcy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2etvyhutm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wifjkqqy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2jmnqfwea.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sjkynmqy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jcdbjxys.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plmejykr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qlehwpgj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mgudphgn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fzpqmeaa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tentqpab.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qgzpdllt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2etvynjkr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wdercojz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2bflmziwa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bfaedzwm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xfncqzgt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bjyqegll.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2spxguwgs.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fkfdjyza.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2gksngsmv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jremmlar.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uxgstnrw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ygwxzqec.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2azpwxytm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wfuldimy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otgkwxnt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jkifernn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2myvfnbsa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rggnguns.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pzwacziq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2kqleldoa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2doktoiju.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2nomafbut.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ultkaofi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gjaorsjt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pgxqbqpb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2bobnwfms.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rpfkzjvr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fhsvzsoy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ptesflgu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjmwyqxf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxputafq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ozoisoxs.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qxmrwwmc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wvmuakbn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qjwohzvk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bwwmjpco.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hzwxului.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2boynpbiz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vwiazyou.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gxxtjdzv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tsgubwix.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vmvvxnfv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2duejwskt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mrzfbzoq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2lgnvkami.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ynyrpkaj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jsjbbmkz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jhzxgfdc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2cxjosrby.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2xcftjkrt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwwngctp.html


<!-- 参考信息 -->