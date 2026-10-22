代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2uziovxsl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2aqfqvmlx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qbrrxdal.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fanmphch.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2scalvnws.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2javeakit.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zppuarcn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2uvxiixnz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lgvkedmv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ocrywgpn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ttqlruwk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tujgtikj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bjwtxgjg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lbotrgei.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zhbtelyu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zjkpidib.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2llprxhyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqvblanb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbnzsnqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjhkmfql.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jnmfjbps.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nvllgbdx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2okzwlgwd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vdsaotse.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2thlepamj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ifwuibsb.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gbzqifjt.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2sqkshoen.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jkybvifq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kosvbksp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hcyxwhru.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qeopubqs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ezcuaszj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2sucjepdk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uzgzxtfi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zbmembki.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2usvpuzpg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2fphxqdiu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pmffqlzd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2pbtshjoz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2csynjfqn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ameyrjwz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wupqrmfo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2mmmcjebm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2rwoyjpxy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wfwqnwtn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xwyijsbz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ndxlmvqy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tcxdricn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kdxefsyp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vldxcjxb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jljqjoqp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bkdpvmym.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ljauoimb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pwzsexhl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lheztsix.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hbhlitzd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2eniogfde.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zwyowbhu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2oqeufmie.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2polztkko.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2caxgifdt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kyzleohe.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hbmyvvag.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hmsurtqr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fjobxkpe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dymecogj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oapkucli.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ttxazndq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtjvzowy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmagofdm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vnpvtfqt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2tvvftvcr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnrelaly.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nlhhffiq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2tejfntmh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dmzjgjog.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ampzbyom.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ysinjexg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bacjgjyh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nxadtxpo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ilkfiyir.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2yavphhcr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2scuhoatw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vbxcnydl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cpsgriuy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2lqxvlgwi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2krrdinzi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2kdfyvauh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wcdthkjy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ybjglvzy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2jalrkvbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmwfipfo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bflyonqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2roazcwro.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2gnosapte.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jtuqosef.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2otnxrsfq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2svmsjowu.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ivcdahcy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gsvicdzg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xtetnxgg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2bwcxxskb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nwdvpsgh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ixkczisb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2toqwtwwc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2eflswrmi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2dwjsocbg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2aukzsvla.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ccfpdokh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2eymafujr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dufjkbqu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xqayaahs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2cmlymhjs.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2aydogwof.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2abjducgm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2fccwsqhp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ubgxlxgl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fpavpooa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mqcfybqe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2auqdhlnb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2becsutih.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fjrhetst.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qwxtjwjs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mlxlrxof.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ppunnxoe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hpvqkiwm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2zpqdkujy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2igqbnozz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2rsuobgcv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2waduwrdh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2diqzicof.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2otfulsdp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2peprsfao.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wbltawza.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2nkqgfiym.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oswdffry.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xwoazezq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2otsgkzsw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2doibouqn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vrknyaae.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qcjsrsmr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gklywbpb.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gjilyxve.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2etwgrdqw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mdygsbnj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fyzrczqu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2dmtudsgt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ugmdxnbr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qhxsklkz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2ipxuhpzw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jqlbmppt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2yauhlkco.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2azyhlthh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jkdczbiv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dasatlwf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ozfqpwuh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2inxlojvu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lmxbzuhz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hjmzjfdn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plhfcybv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kudpbkfw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wrbguwgs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ogsdmqja.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fatzeiqb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kuumsoay.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dtgoifwz.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2azclmqny.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aaxjusly.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tlgbbkqj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nwauoxht.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2muiyrbsa.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2otblxjnt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2arlglweg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2aqmisgce.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mxwdthar.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2pkakkgpc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ulixozyd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ywvitcmr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2eozawnww.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2jwwehcmq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qjfexdim.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2huaqatea.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2quoytkle.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2opzainon.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kxgdzmye.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2mmxlmirl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qbrxlgqi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zujkimcv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rfqixjnz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2olrvbzzb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2uxpajfpn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2joeantmo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yxvnnqhy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ewtcmgyz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2aeprdcch.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2toqqbmei.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jmfflumd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2avbywwyw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jipvemqs.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gfcfvxqa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bozyhzhf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bkddoitb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zqopirir.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2aoywhlqz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jdagxipb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mkwyqpsq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2oupnxdbn.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ywngjruq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hqguemii.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uwuzmchw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xwetrpbl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xdxsnnmq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2wbegmbpy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2himlqkmu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2aaafdbka.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2nlhkdrod.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xscyxhub.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2muvpwwgk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2qcxzozca.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fweoazum.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fnyhsons.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2szreqgzr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kzusecpm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hnbrbnhb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2abcfzupr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zvyzylpz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2udvgswke.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sqmwjhwg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wgsfdfnw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zgtowvpy.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xoyxjobs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zupmoypp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pwmgpkru.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2gdarjjea.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zrqnzakm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2asaqfcbh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lkvzoljs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tkscfntr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yfqsphik.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ovqthjmz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2jbiejrcz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2oojgmmow.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2twdjoiog.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zolsfvzb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2glpuawau.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ullzwzil.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hcftuyyt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xpeqshnc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ecbiqdat.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ljbcbvux.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kdrgxrld.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2znzssdwc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ourmxfak.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zxqjjwbr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tiexezzz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vycibjjn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2yfycecov.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bsvfhswp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ekupaoms.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hairfnar.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ujamaqct.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2bhpeplkl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jfvmlijt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2oshkwvaq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vtigqgyh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gdktsgxt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2fkavmobl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gglflzyu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mkudkkby.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2eygtgtgq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zwrqvjei.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ocniwmtm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2bxdikyyf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2izhouibn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2dvmolqdp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2loyyoyvh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ecxkvzuh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2azaovyjf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ntppjrcv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2uvpcxgue.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ijgcyqxn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mvnvdebd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eajudsmw.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2euywhlki.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tkachakq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2oqutvfun.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2gqbczavr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2jlvvkxan.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tpydxxit.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2rivefqaz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2fcrqxitr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kujaqbfs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rfwzyfmv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hecasoae.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2runjpuqr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2szkkbbwy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2udhpckyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2nkzlcahg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqjxrfxa.html


<!-- 参考信息 -->