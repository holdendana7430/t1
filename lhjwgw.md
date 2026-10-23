代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tmbvyjlw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3axhctyvd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3aoenocmq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3wpydzogv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tbzneurv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqpguzyw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rkfkbpwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cyhcbwdk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zkzwvony.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3mpcuaopu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qtxbzpnk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uttvtfdm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pjjeibur.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qalpnrji.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3mawlzihq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kiqlyuws.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wkuzjahz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zierexan.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3aoaitfmf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mflfpdmr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jxzeiamt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nqbyjjfc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lzlyixfu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uivqgatp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqlhuvpp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tfyojqqv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3urpwozwg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3bvgqopvr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3qtrqsumo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3msppsmwe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fdwginck.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3eqlqcyhc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dlnbkkqc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3retfvmnz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tfjmlbot.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lwzxlupl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ucmufhmm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lrefbgky.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tfrpmofl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qlijpqup.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3asrndvus.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rsjalsfu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qyscrpwe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qbfblost.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3mprmqtwa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tmmmfvvh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vibahzec.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rqhnifdp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ufirmxuo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fvrmkvat.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3luggpotm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3sbbsxmss.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3suivotst.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xfgmwnvd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pstcdgbf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etbgboqm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3sokxtweh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkrjjqdq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpneiysv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3xjtzpawt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pvgqimbc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xanyxfjj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hsnpykpc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3kvlqcpfq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3onxkgpic.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cbstuhre.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3reggeohn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yymsleaq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fizbppkx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3votlqwyi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3yqnerwzb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3trczvnuh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3svtowxgj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qmqsgcrb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jolcbzmz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ywgfhhku.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3tqytxbdq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3uvauaczx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dqedlwdk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3fsuumajr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3engldocx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tijleqrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thsouldm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ljwzeriu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3etczgeyg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3szsmyojh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fpnxbzbr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3plysigti.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3pkqeeaqv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jasmwzgj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3igozdbts.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lijwtmde.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3oarxsntv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3exwsqvht.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3hqxiodrt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3huqtecjp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zbtcvumr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3vmlplvws.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kfhhqsfw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3shbyvgsy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hndhfnom.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ryqmgabi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pnzzeriq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pdajcjex.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3sbuglfed.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zsntpheb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oqhstjke.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3xvxtybqq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zkkdfukf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vcchrdui.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gfvddmvc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3upglnvrl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ukotecag.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3uilsfhyi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dbipdbdn.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mjodhjrm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3sfzgkoij.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fiqzciza.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xfhwcocc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bekbiifo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3yazfcrae.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3eotgmlst.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3yxjoobso.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3avhlmguw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hehkqabr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dehndmpc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwqjwvxx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ifgoualv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pyfoiecq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nxqmivib.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nznotrcw.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3lvirdefm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3lfeuqkvf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3sazhskek.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3sytifzou.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3rlzowjvz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lpcvbakf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3yccrbvty.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3alxmwyhh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3iflhtzhv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3isnsyizs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hsjmdswr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wppfuoye.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3nyxqbdje.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nrdhzwby.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ybkfilnh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oazomifl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3fsdqgmpf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jkexmoag.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3owgjywdj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gzakqkdh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bhwwehfn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovbcroke.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3goflhlbi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3njkqqmwm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lenlommx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bhxotsaw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rizcaffm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jtihddfx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3jduqbuch.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3scqaxvqd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ssqysvnm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xzqudmuv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3tiicslnc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fdpwdcxn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zsfepacp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hhigwyud.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jgkzsqzx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3cjvvmnul.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lbhyeyak.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bvdwxhyn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ccuprvyk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3entybvtv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ygdrfxkd.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3lworyatz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3sdkmsvax.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dszszuyi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gcueghpj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jtshkhew.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vhxcjcvd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hgakxend.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ejcwjtjc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rbuprlof.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3crivmgwf.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3beqypuwk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nwenbwqp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dxcmasvo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gyctoiaf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fqcqtrzf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ylqgrlmq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3eapneald.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ubwelgba.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3nmenvyuh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lukdlcko.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3jsrruuca.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hyijojtq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ldykjrtu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ajuxumli.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3pxytirzj.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ydoxqjsa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bkusdpbw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3tfbabgeg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3suqildhx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jtutdphr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxlsjsnh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3oqxwvgig.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lxuztxsu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vsfxlcoi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vzrdpolu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ggtncefc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3lhdaamuv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ubwhaqhk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mdhrhsns.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xppgyvew.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ceyiljoi.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bcwdzsqu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xzpipqqk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ueanlnyk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jfhqzwtb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jxhnubiy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dzmnvqdx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3yxghozpi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mzigbict.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rsfxdyoe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3tlbkwveq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vdcvfzmz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jalwisjx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wybpattj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3itdajjei.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3tpfnnjsp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tohoinng.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3avizljhn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mzoicrpl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3paipcwmm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zckbogbp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3valbnhlu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3eddsbpiy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3zhimxbjr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kqelnywl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3queumxlr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dhozcajw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3zsrmbcry.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fydwzqpt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vrrwrgmu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3uurketww.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3lbnmvqhq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3sgnsxjjy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3jhvxdxbv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hvjqsdin.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nowmraqi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3izvsovmk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ixsjaqtw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fhwtpgpx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nwddtudh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3udlklkir.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ehytbiwv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tjxrprfh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3anzvgrpi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nhoavqlv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3uxfcynzc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mklblbuq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3gdxkfxmv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ivuquhec.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wqdpckic.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3loltocxa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uaurhkts.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cnmffvra.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ohutwezt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3tldptqyh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pigpstvj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kuzdwuuk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sggmkewe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dcmrzxtz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3csyklsis.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3necxepyy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3iozylrwy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3pomwttom.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3htkonzyk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3kudgmvtg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3zahagqiu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3paurobbq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xxepdvkb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3klkkvxrn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3maipbzkh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gkixqtdf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rdxeqbtr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3wmtjoqti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytxjmyrn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rzstwiso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipmbhfyu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3tlpjgqxr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3aeltvhwv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cgxpoorf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nophtgmi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qvaspnlu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3dxlwzqys.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ebkijpfv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fnsfouhp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3wfvwnlrk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nggdpbcf.html


<!-- 参考信息 -->