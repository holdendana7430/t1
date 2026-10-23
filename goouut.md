代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eimncvve.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mqftaizx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3glxmqcym.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zkkbstlh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jxvnsncc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdftlsfp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ethcpamo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eywbnuxt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lthqkbgq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3fcocnqqr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jskdulvm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mrnyspox.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dyszdqft.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ypkbtcjc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xwqpcsxp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pmckykdx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3hibkmefq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qmgumbun.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3afbgtgfh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bnjsyoae.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3dmxthdqu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lskzksei.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dcnfosed.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3hvhpwiyu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bvgverqo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ieuckouz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gchwjwyq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3bdbycwba.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3teleellj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jfbvydcd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ncuitwni.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qbnntboa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3pjgwawaj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3iuvyauhy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hiojzmsm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3sawltrxi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wifwbtuv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uoaqerwv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ncmltukk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rgimdpta.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3toyrexwx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lffbkbro.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ssyamnkl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yaasfqoy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3sltbnyid.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wffovoqn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qfdebfuo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qveuggrv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xnwhlesi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3aknjqrpg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jzhnqvrq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3vmwmofhx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xtpjlylg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3uuczslbf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3orvafkhs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lpaoobdf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3clvujwxt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zdviyeyq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnziatmf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3unjiimeu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3hlzguxbs.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edjjiapo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3sguwetzx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jkablfkq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3sjbgtben.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iurhxoig.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sjfuiknl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3trqbdyfs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ukhbmrpy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3syzrfuro.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3feqluaxb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3uaihckyl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mvsjtdkz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yrorljkg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3cavqreek.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3esxlvlhs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wiuoaeff.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3xudxjubt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ilvqbalv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xivetymz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quvjlcut.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cgrhjwfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diegkwfi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3inofzxwy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3duoyuypo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3appiuvuq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pmgifunc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xvmhcbje.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3kxplcpmg.html

);
来源：http://www.52xcode.cn/Article/details/gt3tsztdblh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gafpmquf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hvusxnlh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fqgairxa.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3khiivusy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gefbuihz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3jobuovcm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vckfpmqz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ezeigohx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wimqbuxy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3kqzwsvso.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3iwafesej.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3knxiqxpm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dluklndm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hesrgdxi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3spfvuyws.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yfjyhiwe.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3pzuxpaye.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gggckjkn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3przyuyvg.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3eydxbqyo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dkhodjqh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3qlryrgvq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zttfssig.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qbvldrqi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tfbxlxak.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kzgsvtbo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3atmhpmvc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ihegxpmv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3insmhakl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3evkccvnz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3azczthjy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lxajitnb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3potnapwe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3yoqkedpn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ntzlrndn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3cgeshedj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xpahyjbj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3lsyjizup.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jjzdpmxf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3eiglykau.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3dmdztbyc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3exwyqvlr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mnxkepcg.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cnxfvztd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vutffhef.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3jwltueuw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ltnurkbk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3dmeyjnkm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3cavkcutz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3rwmyncwe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jeywtmdt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mtgrajzt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eukbjhdq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cyobwqtn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xppeladz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3nhwuqiou.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3psdvkdhv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3oqaqjtcu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bwreqhxa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3buyprskf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sdwdpjug.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pcwwtmql.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3frnksfzx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3imxfvoip.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dhqopcom.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xxjuxaua.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3fnpmnftu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3drbnwoje.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pdshfjxe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3cohdspco.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fzxmdzaj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3srdbxbba.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wtnzjriq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3otcyiwym.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3chfkefzb.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3vhbapfyv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tggjpzet.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xvxjspye.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tcvofmqs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sadxkihr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3vlhevbpr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ndbsdmtu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3cxtnxzge.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tzcijpch.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3txqrxhce.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ppwofmse.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xowmxtsd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ksmywkuj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hauxbjgi.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nizdjiyr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rpnbppwz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3qkrxvxxr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bvrvsuvw.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nauzamqi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3zimhzevm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zhipatux.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vucjnqwk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3uttiwjte.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3qcgmdybf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3andislaw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3cnmjomvk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dnbwfbxc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3jhvqnrcv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3roauxrfy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bdlcyhom.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3iofmfggv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sdnjjmex.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qiarqwmp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sfqkqomv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3sjpnxhmh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vfwcyaqn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nauoennu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bgrwflrw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vsufauoe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ygwqxerh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3yvadydbt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xwykbxmt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3vaioayar.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3fdrixwbz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3qyqwooln.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kmmuskti.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3skwpewcd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xbcteimc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3irigiaad.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3umogsuqr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gcnixpxz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3booqctqq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3hmnttlya.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ckcmyiyu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3dsjnvcgb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pcxtczpt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mmqedwhe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mcjzimaz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3umhyzvbf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hayvhszg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gnhbwibm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hofnyklq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3geckclux.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3siiamyhc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ubtvgspk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3igutengz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ywonhwsm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xobwtrve.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zbucczdj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ttbvutsf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3chzpromf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jflkzxne.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bkceyqvw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ngmuimoe.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ndftmpob.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3rjenkvim.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3aapwxfgm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3tbvvcvdu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hnwpiwav.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zkjhbeav.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3awvqlzff.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lpftccvz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qhejdool.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xqfsagbu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bxqqxigb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3shkvyohp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3psyfhyyi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qyokjdfx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ztcegwiw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jodowtzp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3dbcmyrpt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3rcsxjpcy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3bbsvnwzu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3wsblofwz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3afwkmtub.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vrhiersq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wygwtejk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uhezcdqa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3zsltlhor.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3llmzwprp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cvvgfimm.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kkolbwiv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yplqyfds.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pgcoxzce.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qxctsczy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ocexahdw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xhbcncja.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3sbofktyf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bjztqeae.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gexfuuhz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xhfmhony.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3flperlut.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wjxdshfw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3hcjmfqsa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3onbiupnt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sxyzphkd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ezaqwflt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aecinuhu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3liagghhy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3axfyvbly.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kwlduoav.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dhqkkliv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdjjxueu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kqvdhgaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kctcdztr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ssmbpwnl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cjmtzbfw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yylvbtak.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3aravfdtj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qytrkagu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3oizgeodw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3rfivmzox.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3hekkvhjp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3iooneamc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3agiltpeh.html


<!-- 参考信息 -->