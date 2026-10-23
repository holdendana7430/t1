代发 wailian999

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gjqufbsv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3favxcsvn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ptakuhsw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xnvhkiri.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nfnfbged.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3kazptzsf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kpqducqw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3silvkwfa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vhcsfgdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejrlcpbn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkcrhdrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lquulaka.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vqvovxzh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3tpolbcle.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kknpblsw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xmvsgynm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jhexdhlc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3czlwpepb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mrqddoxx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zwxdcuuf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ziuouvju.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rksxukan.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3plxojhjs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rxdyxjrj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vtidoxjf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3drcfifoe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ixbqdvxu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3oxbxsrzg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3igyjnwmm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ztqrnhlz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nugmxikn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3uxlqelfq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ontbozpt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cvbialjh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nfkumurw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lfafhjhm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3csujkgec.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tjnddcmb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3uuzxlzau.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ekyzxxhq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3cascyksv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qatfxzlj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xchpwlot.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vzkbkzvg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gxjhshox.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3homguqtb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ebhzhnkj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3iareuytg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hdzedhjs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3mjfudpnc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gokiqjfa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cighdrmi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3drsridob.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3cukwgyhk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3acgkxgmy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3goujzhsy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3cgudjblo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3eatfnxmr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3iocbwhvt.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbjbhkfy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wfflzbhg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mxpnhnvv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvjsblme.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3knwkbwuj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qxfwvkjd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ocdgencl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hnsdnlnz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zxebzory.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3iezedawu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3icdcgqmi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hkwewczi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofvniezx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zgtgbniq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3voavlqbz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mydbpvnk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qrbxnfyz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3sfazqgyl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wazlpofr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vnimqjfq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wnliquld.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3obqalkmf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3oeimhayk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3meacspqv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3alaufxdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwwkbolk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qhclyych.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfyydqrx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nsijegml.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lvhcvjlb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3toovbtim.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3degpwmgp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kikduboz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3padytrhd.html

);
来源：http://www.52xcode.cn/Article/details/gt3fdwehfhl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3hyopqfia.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3mqsjmydf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ivcfflod.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tmfuakwc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3apfgqxxj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ysxshdiw.html

);
来源：http://www.52xcode.cn/Article/details/gt3mmbluczb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3rqljqtpx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3hzlisfdm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ooavifgw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ofsdfwsk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mvpfyxoq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nmtmizvz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3doafawss.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3rgroievs.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3iqruydck.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iniundps.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ufcjtgkm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3epsjoydf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3qgrpociu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3veoiqwvv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3xlhyblrw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zlesezml.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3xtxfogjp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sddaliru.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3poldxcgh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3szbysger.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xekvfmwt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3unkwtxfz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rnolgaxi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3asvhqqsf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3zkwtoxpd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tpxjpezb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3beteqecm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwdkkvza.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cnjbmczw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tejrutzl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sesfqcqi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qkraymwu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3neopuiwy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3uwyjaflr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yxailfxa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3stkzxztu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3aukdytqx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bwvubnkw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3uhidjbcp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3owaltxqo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3urctziuj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3gxhjsebx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cnykftuc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dwhdddpa.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3jdpckfhy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gdcotkfy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3swzosrqq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mianvuhp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yzaqelim.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzjhzqxi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3fpeufnhj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgfljfbc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3gtpuldwh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3boipxeij.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3suekkaul.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3apfqyrlr.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3syeffkud.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ljhejwre.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cstskngj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gikrzfpv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dlenqfwh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3szyhztka.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ywbvigrt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jtrzyqbw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hfvwkwwe.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sakbhpiw.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cebelhzt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3gsrxilti.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cplkctlj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dqxuarph.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3beqlsojs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lmidrbzl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rgkuckqd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3evhfcitw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3vtticxjp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3kownszjh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eabemgmw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3lxmqnpuc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3idjldyyl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jquumnve.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3vdehrimq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3gjjvvzoz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3smvhmzxx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3pmghkazq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zfqhrxvf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3frxxtbxt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3wppqpbxm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3byzyeqxa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3tzcafxmq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lfnnbfgi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dhljehxq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zwaprjqa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3smhmbjiz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qrautdce.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zatmmweo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3finvtpew.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wppiqgua.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vcqchjoy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3noujedaj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ifktvwhk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3uaydgzdq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nynmamxq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dwncoovo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xtgnejxp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3diyqtlca.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kdzzbfsr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3puubgbzr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nirdzfrs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vqykmlpk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rvwrsbme.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3owqncuid.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hccobjif.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kgmywsrx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dhltihpt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3favnsfoc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rlqozfcc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3njmzqyil.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hlakndfa.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3xwtfjwir.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3maqnkhxp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jdcolibp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pqwnefzy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3yhwimrzi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uxbulcly.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3unkjczbu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kfdlzrgn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ykyvoxyw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3dmsyebfm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hjsaxdvx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3rndxovuk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hsmepnyj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3rqecudhd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3rgnyskvx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hjpjgtit.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kidxufjl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3etymgpot.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rhfffmwe.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ymutxjog.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yeeokpzl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rgyjasqp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3wimjvngt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xbhzuaik.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3cenvauph.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fkcrucpx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gykcbfht.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xednprna.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dsugulqx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3sxnjwjfl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3earcygod.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fjszjdcr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vmlxcvwp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3woxbmepg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vkabybvm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dkqenmlz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rcavgbti.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3bhcjmxcl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aobgqoms.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3chggptno.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rokpgiyo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zinigcdf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rbklwnry.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3hnafflph.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qpebynkl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3aoxnzymp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pmbxfbbu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yhvjntia.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jpmvflho.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3reojlfal.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtvmjvtn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3biwwmsaq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nzfonwkw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ftkuwmim.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wgutjijf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dkdepjjt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qdqlwtqd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wfjbxwzq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jcptczrw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3aaedhxpq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fymwetec.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qdrbwdul.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3yjxgaaeh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3bgksdbcb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hyndklgy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3pvnbeocq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3wlxfusvk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pgbgfydi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kjvbtqqo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rmwklsny.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3pmillpas.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hetkxomx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwdoeaoh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kzhxhvwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtlngjrq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3sgplwamd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rcqvyohq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wkmejcal.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mpbbistc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3sksnzaax.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ucdhzubm.html


<!-- 参考信息 -->