代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3mcqygtva.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hevlsgnv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jupntgvw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3yqdmuhnf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3huiagapm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3aboqdohd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hypkmvji.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sasjvvqk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pwzgedqn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3knotobhe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tcrqctpa.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fjwuuvuh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3cmbsrvft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyfgemkm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3akudmiwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdeniphd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3isetstse.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lvhrsxfi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3fllgepss.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wplxekvz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vdqpxuhp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mpeipxir.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vawjtaow.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3qfwqvsxl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xlbdoprg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3korgouin.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mukfacec.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwouoacg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xdgrnods.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rnvjvhuk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rzkdnfqk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qldprwbi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3naylhfjt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3agvyoezy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3pyiteukq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kexptqrl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ksupslgh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ypxqccye.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mfoylted.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xdgngvld.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3buiwkypo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3xhirsbzm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gllmgegs.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cinnsrmt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nxbilljz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3txsafprz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wqxhemto.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ffjdjsea.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ouurzxxh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mapiajer.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xaeeuaol.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3flvqrfoi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3tgrxgtkh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ycupvmfe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kuiljfvc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3mscapays.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yqlebbgw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mreepwth.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nyfilkyv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3iilcetcc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3rydmxkfi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xqtyyseg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lhkytole.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxcarvdd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3okuwsesf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3okyziese.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sgjmcexv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3aqjcyxmp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mbehqcap.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjoqdvta.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hvmuttpt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ctvwzttr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qgydmsck.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hscjabbg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qcyncavi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3vnqivjfz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ggigawep.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vzhuxlnr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hcystdjm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vpjknsuc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pqlbxcwd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3efwvfwtq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vlouzqlm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3drmksfil.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3numdjwbm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jlyxuynj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kmoatxbn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3unuabnlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txtrqhig.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jhaflsof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uigjcwmb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3vfufsnsu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3paopgttl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aegclfrg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pqdsptiv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3fbhihwhc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vzzylaks.html

);
来源：http://www.52xcode.cn/Article/details/gt3dcxtgqub.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3obkxteou.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3izurnuya.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hpsatqmb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nloakxze.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gviumfrt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3fxgrijnc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3anqhcqlr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3gbbmregp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vpjexsrq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qtumsmsi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xrtctmyk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3hsbtudui.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3aoyexzfz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mevshipl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mvviwxbv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3zjhudnwm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jblfsmpg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3syfnythf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3syhlggae.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3veqkkrnk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xsmzujvj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ndngsdxc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gyczvfsv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xdipvbjf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jqlspxdx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3orlfrrxq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3pjkdmuah.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3kuhlmqpv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ttqcflqc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tyenjqgg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zdfixzpo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3gaaevjpd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yziodvym.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ojsbksol.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iyqiepon.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qzjwljwu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jgczjsqz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ahyanbbo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jbyizgwg.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ivymywbo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tcyqzlan.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3azqzdeqt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3epricvbi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jtzqvunl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zqlixubp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhfztpqd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qsruwsgg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3grefxkoo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3wxfcgvjp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3byuduvqv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3trzrqxlo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3koablgsn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qzyvihbd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3lizouivd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3xzigrqlc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yqoinhbc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbouvigd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ihrhyyuk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yczbxbtp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3scvhrrdg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ablgkejr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bozngdmx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fnjqgwyw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kcqdmnla.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3galtkkys.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bxwtfpcd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xohjqocn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ofhscnop.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jogcojdm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3cpoudfzi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jnenznkj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3aqlsthbu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vruwnbgp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kdikpgqw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3nsrtzoiq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gxmpjcjx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kdmdwhzv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3tcswzmru.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3egfqqrrp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uirkxtqh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jropgpfq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hbqvgcpo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3uymjxmtf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3fcdzokav.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ajwynazj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nsiiztrq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ospabfmg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3pkqwitep.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ecersswd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gocsxtlx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bnuqppfa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3zmstyomn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ielxcfby.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sxbhzker.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3nlwatiuq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3udlnxzpf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3stqqvskd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kvaagczi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wwzmjfsh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fsuiaizj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3icxpufox.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qobhtlcb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3inavkpxl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uzwicdrb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bwmgrqaq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3udyyycxt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zefvtucm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3bvofriqi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jzpxesvu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3sexxuqnw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wtwzycff.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ijkyzakh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qpmogmsv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xnzikejx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mcfpfvxt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3vcipfrnf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gdejroxr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3beyyuzwx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jrajemdp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3iqyfwwqq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wnjyrysk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ozthhmhw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mimbfsyk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ofkrevup.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dccmtqab.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qfejlojn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3altzrcsp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qtsgijxx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3owoikdor.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ttfnyjof.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3isvtvpyx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3socimlue.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zwcwcuws.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kwpxzorr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dlnfnttm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pfbhshyo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3sblmzkew.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lhzrnety.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3iyqdaurv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vofvbxrx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3gusosflx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jddecavr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3zuhdkqmk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dyyvpvoa.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3emhxmejv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jwinhnha.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3evifssid.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vltvzrwu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bckjneay.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zhcdxewf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3inpwshen.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3xjveoujb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bmoewvor.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3zgyqznlo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jgqfzbnq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3twbhuynt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zkmdoecr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wlpokgtj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ujgtcujd.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3cagaoeuo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3bzbzhmdr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3wjwuygux.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3laefduds.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rpmgnktt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wrzuotcu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mkqwlijr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3lgbvxvbb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ohszfsih.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3pydzjmwf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3cjczomos.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fmzhcapa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3upfcponr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rdbghuzp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3sbozqgxt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3essdanpz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zbweoqyp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ndenzgok.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vuswyrjw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3ukhpppgs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mfdfnxbw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bmdyxbrj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ocxfclom.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jxxnrhyi.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yktytxwi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zzcxgadi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3weyqczqi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3bwqlziua.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ncuntqmr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3qtyjxvyl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3bgyitfdo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vpuxibkx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3iumgluqh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kkcvrpqz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3uehybueh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3emoytfoe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wcqytuzo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3plupgsfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vofrwbse.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3amxocdac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebqxtxnl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pomeollq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qiksldei.html


<!-- 参考信息 -->