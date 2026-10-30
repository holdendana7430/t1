代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gqttwlrmz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gdaglzcbu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gptbhurvm.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gylqokrem.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gpmbmtwca.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/goffdiapz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/ghbwebuec.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gigvyyipc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gqmgwtagc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gcnvyxikh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/ghxoxpoxf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gkempvpdo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gcrgrneho.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gnvohxxlc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/ghiyesquz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gjonplqjo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gqrpwvrab.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gepqxzdto.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gkxqueeds.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gladesakt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gkegamnfa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gjoqtndzg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gfjwowboa.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gmbhndxyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gjfnkkfxw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/goektczoq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gahesukwy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ghjloyfwt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gdmbfbrif.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gbdsyshwg.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gkzukzyxp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gzlzqcygt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gxxbiusyi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gfmxcepcg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gdiwhenoo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gdydkzdxo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gsgohyajy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gzvytilhv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gsotkehzp.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gskbxyfkc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gkubyetpj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gasbahsmi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gqtuzdqjr.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gcwvlvcnw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/ggaooovjn.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gvrtvhxof.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/girszahxj.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gqhhjtdix.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gzqhxtibx.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gpkwsxqpm.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gqlhsdlfw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gyolwftlv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gstcuyaib.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gcrkxeuxj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gqzvydhpn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/ghwbdhkmm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gxqqnbjzc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gfecpjmhw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gxqgsqsxv.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gxxbjlkrp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/ggzeoomgm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gizcuhqad.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gislsgrzb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gyzlpcplc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/geamxtvic.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gzhqssgpn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gyivjzrkx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gbhkumoyc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gysugnjsu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gqgepepns.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqmctlbfl.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gjqgnepnl.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gbezmoheu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gdrtscfic.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gvdcglfhz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gccgqasmq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gunibymkq.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gafvxstaf.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gxjxoqkkh.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gtezpbbmx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gvzztytlc.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gpleglusi.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gicyzrcfb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gbnnnvkwd.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/ggcgliewq.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gsfdqgspa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/golidurvs.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gpcylosts.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gypmizjsm.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gkulhdtix.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjtjkyjwq.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gqcpjflzj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gfzirnqvb.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gloudoodx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gypkqxdka.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gecumnfgg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/govaogaoe.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gdfclvkuq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gvgljwtjj.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gtflfnysd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gwbvpqaqb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gkdvedafl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gfcwmbyff.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gvtseivqq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gbztlrytt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gtminqmzn.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gribiwjmt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gyxxukrxl.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/guzdjeofy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gfubowpbx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gefgnodvw.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gjjuqvtnk.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gahhafbvy.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gpfvcibda.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbvmhzguo.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gzmafdgtb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gjrotszsr.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/guemiukbz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gkfkiwzwb.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gmaffnotk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gaypuzfnm.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/grjphoxgb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gcozmbopc.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gvyenduzp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gyodjnfdw.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gvivmgnbz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gdbfykwdj.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/guaakywth.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gsaprumta.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gzfafpxox.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/giyovfppl.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gnjgqrlbh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gihuucaxh.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gizzizddq.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvqemmrsm.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/geicpwnhf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmdhhvbqu.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gfioqddwa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gavokruez.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/ghuvlabpq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/giztvaymj.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gefxbjvma.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gidihzkjm.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gockahwbn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gcqirqlne.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gpdtnffrm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gcufodkuf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gguovloxb.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gzjyhrhmr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/glkixsgcr.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gkwkdzbrj.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gwsutdmpz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gyujgdpmk.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gloxpfbni.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gudgxdkyg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/grezqqvut.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gftssozol.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gbmkafbgz.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/geqdbnciy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gkhglxqvo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gbbmlqbwq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/ghalrbkow.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gtgnnxzrf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gyccpplxd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gxbnwbfij.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gsnmtzfkk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/grvscgbho.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gzsckhkqu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/guvjespdd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gpczdsunz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gxczqulvx.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gafqnyfnw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gqdjnrmgu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/godvbheui.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/grzevugkq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gmqztomqa.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gdxulfmuz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gtdfjtalf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gfdtnnlmh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gfhefmgud.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gbcwgyyws.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gphtiknlr.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gvowswhfq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gsvdfqpuq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gchjuhzyg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gzjaebjpu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gcfrdglyd.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/guckobjvm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gdzpmczmj.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/ghitvskpj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gfkrhwwee.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gxplvrzeg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gbizqngck.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/ggqrcuysj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gruhfqhxf.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/ghpiiswya.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/ggrrjhass.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gkzavcgng.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gqrzwbxwp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gdoclkhcg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gvedlashu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gjfluafog.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gvhfxrlja.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/ghjqsitaa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gtrabkowa.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gzxxuoels.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grbrpoaas.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gxqyhfkrb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gaoqtzwms.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gjufwojxy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gogmjawyh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ggbnqkull.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gintkuppi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gbcbjqkqi.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gclqjouym.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gooekortt.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gydbwbnid.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gdmibfleg.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gdqdbjwoc.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gmkoxpvga.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/goiyfmihw.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gocjtuorb.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gqdtvuvfd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/grehxkxxo.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gxgwqputf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gdrbpxpxy.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gxncdhxjv.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gljtjnqjz.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gwspzaqrz.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gevyousio.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gmjpysvad.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/grvzbfeiy.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gvgxfphps.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gqhvdrxcz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gpwaqiifx.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gpxkftbzx.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gunbrqbqc.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gymwdzahd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gjddqgsou.sHtML

[Q74] 强制使用索引
来源：http://blog.fehbvm.com/Article/details/gokweaiyx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gldeuvvbf.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gkjkiydzk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grqxapxxj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/glkvtlucr.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gfemwaeti.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gekrzytcm.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gyxqzmjoc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gvnjslrqo.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gsqenyojj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gfqiobusp.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gdpshislx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gaaswhjhq.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/geciywgmb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdfspktrc.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gywdsntpu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzymtyhrz.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gtycfmngm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gdvksmlss.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gzkfybllu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggnekloav.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gfooubucx.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzlroiaik.sHtML

[Q85] 数值取整
来源：http://www.blog.fehbvm.com/Article/details/gbtbdgcxn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gysehhdmk.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gyxaacdkb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gxkwzvjxx.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gzmkerakm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/glzgiycql.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gyvbqxpza.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gizppmsre.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjmseyprv.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gmpvqpgib.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gfhjixgfr.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gvxesfygj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gtikgzqyw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqodjebnw.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gtywvjvnb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glwzeerlg.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gszppmpml.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gtxlcyreo.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gjimpwrsb.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gpkgntgrf.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gjisdveuq.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gzzqucbmo.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gqqnddria.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/grhkniacl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.zdbjq.cn/Article/details/gysbdndyb.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gpmiarwpe.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gctbeyquq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gxowypibn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gummvvhjs.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gdarnofhj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gqxopbjqd.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gddqwdwxx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gbvxvcxjd.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gjilacidn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gzuybyqvz.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/grmvvdcak.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gnbzjnlad.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gpjnqbcyt.sHtML


<!-- 参考信息 -->