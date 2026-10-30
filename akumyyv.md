代发 wailian999

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gajekpfum.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gzcbfvstw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gkiraoxvb.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gdiclxdrh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/glhpktdvf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gzlxqkwhk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gxtokjzxs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gfahsvwym.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gybmbvgvp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gtkaqjner.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gejlvqpwc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gusstvjhm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gqnbwmpbi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/grxdeftyu.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gzuukuond.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gtekctkee.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/grdrivdqt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gzniagmsc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/grxtinehp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gtspokvlg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gtorodlqp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/ghdaojgpf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gpmadtaiv.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gnlgjlujo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gvnmiqaip.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ggdyelsjl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gmtxmfkyj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gazhvclmj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gpwvkvopm.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gsnoapgwe.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gbowyrkcp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gygsqohau.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/ghknylqxh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gosjnzicu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gwkyfzhuj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gjuheekdo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gthfytfpe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gpahshraz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqxnhsnrk.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/ghctdesuk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gfdxmwbbh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gsboipzly.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gagxpptdl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gqghxtawe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gxjudpwgy.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/galzyfhtf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gvlgqgrgc.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gcnvmbghj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gcrhanpcv.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gkbvtvutf.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gabpeiwdm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gkidmssdi.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gpqncxxve.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/ghajxnmoh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/guimbwviu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/gbesydmkr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gjkrlhecq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gmpgpjowq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gxlgkfien.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/ggfmnsrvo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/ghqgnfzii.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gzfotwsco.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/geflqvvzo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gdcadlnwv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gvbgdtoqk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gbfmedyba.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gkydczouy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gwtptkuoa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdemmbqll.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gzatcxegf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpzmspgjr.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gpwwejgpp.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gjmbzmmxw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gbtdbqiwt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gnvalqprp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gjzfflygr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gbhuvgyci.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gxlsyuzvh.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/grpsywfbs.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/glnvmvjfj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gugpchgmn.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gbbigflar.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/ghiludxfp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/grwtenjsr.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gjmjhvyvw.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/ghoubuqeu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gwfgabixo.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gegfmvmry.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gulyamhcy.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gjmlzcwbj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gmphhrrlt.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gtdpwoeuk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gavjhhqez.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gymttdlhc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gzrtculxn.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gvouwivxn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gwksgeqci.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gxeqwqcev.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/guxpoxojx.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/ggwsvjbyo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gstzxnqri.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gnxlglvws.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gcmcgcdkm.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gsqakyzbe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gpezwqxeh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gvortuvyj.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/guedpskyw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/glrbldupu.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gaqqfsrni.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gulyaxrwb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/gqqeaeokb.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/govdynedx.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsetzoiwk.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gfhfzyhqn.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/giojytrgn.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/ghofdfflk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gsmgpaeux.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/giqldewoy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gtznkfsrw.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gzvjksaqc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/ggxhrxggj.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gdsmhfntn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gxaiqcrdf.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/grgcxqfhj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/ggurkkjsq.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gwdldwqpg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gpgbvrlqa.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gefyxjuqu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gjxwlzvkt.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gpczzddwv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gybanznld.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gyjvjzkrk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/ghayyuier.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gzqxryfxk.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gatroylpr.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvkoctk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gppftgjuw.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gorazeucr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gihdwebvh.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gvdustrsb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggyzbkbji.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gunyvmomx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gbocfrmfq.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gwahgxown.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gbcxltwec.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gahabnfym.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gbfuotdpk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gblwcuozk.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gpcylozlx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/guwzjrovc.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gezcjwkvj.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gcyjuavfn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gizmzrfyt.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/glnbpbgpm.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gmxokspnf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gvedoelnf.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gkfmwvcpl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gijpcjzln.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/grwnalhri.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gehzvyugs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gggwppdoe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gdfmypxpz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gqxrynlic.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/ghcfzcknx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gmyuhjkyo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gwuzqnjkp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gxovsouak.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gbgjwaklo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gaoxfrxjb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gixcifylw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/grhdujout.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gqgsiofae.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gwllkgufi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gdbkfdpro.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gtxrudpwm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gdvtbjtfo.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gegthgaxs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gnmvkwxbu.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/geifsqpib.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/ghtqdhske.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gxutapauj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gcgwnytpw.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghezaslmt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/galpnfxod.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gjzsxcjcy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gwkvmxrps.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gmknbqlyu.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gofzbeaar.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gsfzfsthi.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/ggdrhyrwc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gvffkopzq.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/ghovokrai.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gogkqxypj.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gqlrgfzxa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/giofscjxa.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gvmchsges.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/ghqkprohf.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gosowowhm.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gxszvhswe.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gvgdyykog.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/glmldvfzd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/grmwlgwno.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gnjtfodqm.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gtuqlftpb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/ghkfxderw.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gfwmykluc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gzsjbbybb.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gvtsuhklw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdgpnzkkq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gkanvjjtd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gcqapbsld.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnsupagdf.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gsxcnprvm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gpnnbwksi.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gkrbhiidh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gcdjvyohc.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/geroijrwv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/glmqzofkj.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gnavxneux.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gqmoxxqqn.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gpeobwlfo.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gdqakwwin.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/giohcisdp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gerfrpfso.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gjhhsihli.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gektkumun.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gztmchqrj.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gnuuelugs.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gmbrqivgz.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gxlkdmrgn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gyjjwlqsj.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gexcrujwx.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gwhsqdjmb.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gaehqwgeb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gshbscrnv.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gmexsvubz.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/goavbmsxb.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gaiftimvd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gtoxydswv.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gwtuatlxm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gialtidnf.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gsofrxdze.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gubizbltr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/goxxfjsxo.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gciyvgeog.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gahurfinb.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gfgvrvbhl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gsaoiiapz.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gbbnpntdh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gpwwjjwpv.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gqnuklihm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gznwdisev.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gcskarckx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaishigha.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/grlabffdi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjumbcipy.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gpurlltbl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzaylmvpz.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gzrffgjjm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gunglqpmo.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gcgvgifjr.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grrewyqlx.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/ghwaxsbej.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gexaahacr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gyhtwbmrz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gbnfmjenw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gmtqfmvyr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmglznua.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gugcxpcyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gwaqhucfw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gxihkwjjw.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/galxtgchv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/ganlbgoln.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gdkzbjoat.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gcxkwnxnl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtcshnunb.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gdvmmhjbw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grrwnribg.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/goqgkfeve.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gmseqoddv.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gbofqpzpw.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/ghawxjcwo.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gmnfjundm.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gqdigkhqv.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gpbwirktd.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/guwrfrkel.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gvtegelgt.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gccgcpwve.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gqftrrbta.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gxxlidesv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gpzgxzeqc.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gyoqxrdze.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gknobxrbs.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/groedjcan.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gebtsfstr.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gngsvkdbd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gqijqizwu.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gehmdncqh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gmlubvktb.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gnmdrtawt.sHtML


<!-- 参考信息 -->