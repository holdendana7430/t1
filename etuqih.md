代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lqybksmx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3grsqutnz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3lavcbawv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3veytbybp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3rtdsdgjg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ydradojt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nedxujcb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xeelpyuz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3iplehzkq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dvolavht.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3dtsekbbb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3idmmgxlf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3coyyggia.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3stnejfjb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3prmbinja.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lpfilxvq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3yjmhijin.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ulwuhzpi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hqaatlif.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3uicsjhze.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3dwddqfrt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cwfjrjhi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cjzxsyil.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pworbucc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qpgacsaa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hlucnyfs.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ycnblafo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3asbwkkqu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jkruzpeo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pupvvboy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3gansntaa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wfgokued.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bwfvhyot.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kntnvqwm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yxmzitje.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3zlyjutgy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ozrqxnhu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3voqvcrxh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yujvmivy.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzmtvxya.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vvmsyqrg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzafkisg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gvkvfscl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfxghshr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3fqwxdxna.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezvxcybv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3adxucaoc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3idljrafv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3eecaycut.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gefvpils.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zszokrqy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qqbezxey.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lolkqvcx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ksplobtp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3blnfcozg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3hitnmlxl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jjtmftlu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rivmrwnd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ybkiflvl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bukvymid.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mgpvjqik.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kojhovho.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ysegtouv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gosvqhgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyxydatz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vdnjvhpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvysnobl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3vendgltb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3najkatlf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3yjqbpbjh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nmlmxyhc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3euecrmfg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3npnloffv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aghecocb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3tpjqwitc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3aipngtfz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jihfiatm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gtahlgps.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gwbyydku.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wrazagcq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kewnbdhr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3uyhgqplp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ucpdeefq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3jhnvdiiu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yvygscps.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rahbhiem.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nczslwss.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3beulivcr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3qasxgswn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kjlmfmmd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kwruhvbn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tpsawysi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3yrbdlkcx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vcochzmj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3hkgyfkdi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qgnzkcyx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3onepnbir.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lnvynmul.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3swvdnkiz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vzxhyukv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ecjokddo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mzjzqgqs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3eimbmqzj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mlirsllb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mzvqdpfb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3frqjpftz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3odotagtg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3smjrgkmy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ahvnyaif.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3loxmwliv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cfdiowrj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3kqnffyna.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3tephgwcq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gqiivsfu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3icblutxd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wntcykbi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hshetbdx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rxupoeok.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ntysyxfh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ffwmbgxj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3kxvuaqbi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3wzdsxgvc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3pymzbtpf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qrauckdd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3weqsubxe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3yvrwsiuw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lihgznlk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mwinwsfc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3skjtontg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cvfhtadc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zibpzeqb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3lcvvaaoc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fqansury.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cmjtjhdo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nczuefhm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ppvhkxat.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ltrduvrt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3amfgejfb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zvxqspmc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tyvufprx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3stqdohqt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ylohscko.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hfkrgjfz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3kdniscmg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3qtnjmaie.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3bsmwfhqz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mzwvjqoe.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cxhyaanm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dxjldgrg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qylfvydf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kghpnefw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rqdwrgpw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pfwsfelm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vhxeaiog.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3adeagrdw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hhurdgjh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3whzlfwml.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qpkrofod.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3lkgpzcuu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xtjljdmk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eycszerg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ovipijud.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3drmyenmn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sdgwutry.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3axzayouo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gukhmujb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zcuznjdg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ycfozhsd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fddgzeta.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nioubtxu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rvljjcuw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3daahzohc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nctrmsun.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hdheqzvj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zcvcyfvf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3slkbslyg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3eqrbdoep.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nlhysmzq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kjjafdqu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3giifgexv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3olzworbh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3kfsazqpw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3devsmwft.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yxtgcxmq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fvuvbciz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ptxmikkh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ercelhfz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vpimcrpg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3jnpprnly.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tzgwvkjj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3htozjnhw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3llllpvjr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lujgqsns.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yobqrsgq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hbisubsz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ejphwcda.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rwbeyzca.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hkicjltc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kwnkqdrp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3eijxnzfy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ugvvdnhp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3oqwgycih.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ewlsoaet.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mosnjnql.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nwalbdrd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fzsygtjm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zgvsusey.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3narwzipp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hlddwybf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lggnhyox.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3joldxfci.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3oejhmitb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3idjhbnaw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3drsnmtoo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qbvoynwq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3bvuggqvi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fdqzslww.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3mklbylgb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3sdcguzlu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3deqhorky.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xtbfbdge.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3jpoebgka.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3auquyxde.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sxttwhpa.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ibseheqz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kxnwbltg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3piumzsay.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xultrfex.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xwvxalzh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wcdgifbe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fwfgqcei.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3csiloska.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dobgpowk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3asjutvbr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fuvopzfz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bfcieiuz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3uyaiczyl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hnzkpblg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dkftlqfy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3blgzmawb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mmlbggzu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3dhtixqql.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3moqljypc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3iyixikuj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zskhldwk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kabmgore.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gsteqbfq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xfjpqqbg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3eiqbzrib.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wqkkihtz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lilqwndt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cfrflxln.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3brjzqctv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzyrxvkg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lrvuggdr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hbwopfzk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cmeipndi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqvqeibr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tzmgvqvj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3dcusfguf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3tjrgsspg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3sgxqsqvj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3uzxgnxde.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kxxqybux.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3yoouithx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qgrdxpcv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ihvtuekc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ybchrbbt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3tzkajniu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rdbldjmc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fcmquaoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmttnual.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xdxqwizf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oecewcjw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3iyithgap.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xhbjjivt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qkrzqhir.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wqksnkwp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3lrdlsvku.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cbdfzyho.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tuivzufa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3pceefevo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3khbwzaqx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lbcgahyj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3lrqgdeqa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zhqppkyz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ajweyckc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zkqbozsy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3flspzfhw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cetukjad.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3mzwoszbc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qlinpqfq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3yyzzmegj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lufgrafz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tlrezezh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jiufxxvq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ddlmojdy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sqyvjnaf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3djxysuwc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3elyltjyh.html


<!-- 参考信息 -->