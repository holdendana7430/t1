代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zkdldrzv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3bsilwljm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ujdkfubv.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xyhvimow.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3amfbfhzk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3xvdticgt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3llfhelge.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3salgsuhb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vxlscrba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ankzench.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppmjohco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vingeiwm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qgrbofdc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vbcrzzis.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bvwbqedb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ymxdnyry.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xhgkknvc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ldnzzrvh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3lkmteuuc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wocznxwd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dyzdsqol.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jpdyfuio.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lxhxuekn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3atubdmav.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pdlslsbo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wjkwtixv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hlyfilhu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3vzbhltlk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqapuhkh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yyemgqdt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wwmenqyx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3iqfxhjxn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ffksdzih.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zrpthavg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3evhjhpeu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xzlmvsrv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kfmgwdjn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yafqstun.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ftizqcva.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3isgirsjw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qtgdxxvh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3akxryajb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vhunztxb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3catowlgj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ptcvsywb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gzacmcoo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qyepvhwh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3wpwwmkfh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3tfhyodwz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jggotxuz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3fqwqjpkp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3rtahweew.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hsizdsys.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3pljoikyf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wzvwelna.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lbokoixd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3wizoekzp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3oecjiuey.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lvaudffh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scvalwct.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3crbldkuj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xrxubdpf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3afflvrdh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezajzoky.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vtghfgiz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntvwcdea.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3chghvdcc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ytfadyet.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hnphbawl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3adcsgkct.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3akxsfuzv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3tlmqprjl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xvdweeny.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vvhguxww.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3armcbusa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3azebwnxd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3aiekffze.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kuwowerc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3oboslrsc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3eqgbpqqc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lparuqdd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rojtxijh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yyanmsvb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3fhfbujnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msihujbg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3vmnepgly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hupugklx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3uvmnkrqt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3muapsyuz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qevbwqic.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jlyzrsjy.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wowarxeo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3gavpbsqs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cmldfvwq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3pedurclc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ksyifqwa.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lhqkkuuv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fnklywwl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3gcwpsian.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kefjdrmj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gccxojlt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3drqewemw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jmbhmhkp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3aeugttwf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jlzkhkpc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3klbudkqy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3xzhhpnin.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3pnpyfcdf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gopepltt.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3uzleujru.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ndolbfdt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zlehcsvz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ygifuehw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3djmoutkq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ubchbhvm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3lmjqlypj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qrxgaqub.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ccrhtxbl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ijldbici.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kvfxnfhd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3kjlgvxhm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3znfjbhmc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3byyctbis.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3eyikgdqe.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3gbpvavvk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mnxwvmmm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ucayxkhc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3bgbkdybw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pwbdimgj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xdfdiptx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywjzgcnm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xiidwdyb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3vourtnkw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fkhjxyqd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3cmoywqqq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3tsoaqnul.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rcsbadoc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ndzzfzen.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3nitkwzsk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3vzxrlavi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vlmuojre.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fdhhkbmi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3fnmxvjnt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fsaclhgo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mrzonatr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3kienxicv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwmrhoun.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3tqkvmvej.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mtezbpej.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cbtkxfif.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ficknign.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wnwbzyje.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xcmwqlkg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3txsyucja.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yjoxmoqy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ijzxwxqm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxbqqptw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fciedjlo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hexfvvdx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tiikqjcd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ugtidjvm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iquevlmk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rgeyuqgy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zouoknse.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3mugillfv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3crhcqdnt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qghmcmzn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dkbmdmco.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3aiuitrna.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sovltgbw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3eaodnjoj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ranvmgay.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3azbonfro.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qgaaqcph.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kfiktowl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3kwijzulr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rpasmvmd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cxzcfukf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ieevwehp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3troxvlce.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cesreqqx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gaqqxams.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qykjzpxi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3hzlcyzrt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ppwzvcsi.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3acunsjja.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3qcajlnhh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hvhipmaw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3dqfdywui.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ypruoivh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3xdowrqhb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qcityoiz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3txksvrmj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3yqctyrja.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nldotpse.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3lxrekfsn.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3dgamrvae.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lcnibizf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ykpohhhh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3kzxjiaxa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gjefnble.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjdxfly.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mvugikml.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bylhqzir.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wrkubwtw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3unricqzk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kxwrkkkh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pieuiule.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kdantasa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gdiktsly.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ssdcexha.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vsfjwgic.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ryisyjnp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3dgnwmxbe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cfafswvg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mpfhziwt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qzanutqx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pfpfnfrq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3bjfobdqe.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3cddqcrij.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3alfunqao.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mizdlaid.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lsngsume.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ifjlaltb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kijbsacn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wpdlxjsb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3flrtoewr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jnnmlygi.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ksrwepoq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hmmuqgve.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qhdmkuvo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rqptzazj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vzzhucej.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mugcfmdf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ionlzuct.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3osdjuepy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zmbcocju.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yxwxiznl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jhwojuhu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jfgyklpo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ynbdtvon.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vjtgoehf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ijztpufb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vhyeoneg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3hkquzwwn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3oaqstbxp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3cpjhpsea.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3qxsyglke.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3khiellee.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rjcpzivd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jwmvacbz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3neddhlai.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhdariwo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3cklyskzv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ympmcuvg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3zsrlgwvd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3eseisaqc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qxojthze.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mpbhvxgp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xktoaqbe.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3euynkpwt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rtzstnnf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zrtgbgyc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qcarawsk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3xgjyghfz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3pwcvttue.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3tvcenrxf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vljlalsm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yvucypnq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhuisyqo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gdbqjafj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wxtouxpt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3rzezufps.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sspqcuyg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gkorctvq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dtyohmvw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qrsvicvv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dmshxxzk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qxumnkyz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xofaoztp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3vihvuwvh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wcnpgfwy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3tislqyex.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mfahkchw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3fioealuc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ubxkgfcg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kitsdzlm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wsfylfhe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vfxhiftn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3erfrxlvs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rmczzxyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhxsutxh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3etecmplu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcpfpgvw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ltynldau.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vvmpmymp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qrzrktiq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yllanwpr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vhicjamp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ftbvgulm.html


<!-- 参考信息 -->