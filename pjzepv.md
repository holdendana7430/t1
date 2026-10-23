代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ahuixhuz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wtnsfbkb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fgdsiwci.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zebkgruf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qgknxpuj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3scztwksf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xhnvjmut.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cxlvdajf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dquazrta.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wfvehtmr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3uajzqcan.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3dtsfwmqz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zioohnyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fadubnmb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3atrtrddw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypklqjic.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3srhckpmz.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vujtwfph.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kpairkvp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zjjlnxlr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kfohtfoz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3rsfkmixl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hwvajmcr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pdrrqryg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nihvlayq.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gduecxzn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3mxtdcqbm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3guztwsam.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uqoplyke.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vscquksm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3unytmqgx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ymuhtaeh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wfqmuqmo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3mijuquno.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3udifrofe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3bqgsqlob.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3edujiyiu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iystnemw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ijaroiit.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yhzvbjxa.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3hemvwhfp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wyfucxne.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ngjhtcgp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fvninfen.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wjbuxsur.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kdrmcdua.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pouwrhmj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bkwomsnt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gdblduob.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3pucakckj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kxpiwton.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3weogwslp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3uaqldjlq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ketysnpd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ybxlfxqr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3aqmxmvlg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qjhbohpe.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vkpmftfl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nlsnwqpn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yougnqtl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3tqrurukn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3iwtqubms.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3lpirfpfj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mpegdfjr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3krchzkyc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgzewsph.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ypdyyacb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjopnvqd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qbnrqgqg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uapbonal.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lcekiaga.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3oeeqwltv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3hpkcdxtq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mnfiezuh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tockgijd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgsmmupr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ygeidgfh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yksfbvdw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3geoamxpc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3urtetkfq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3plvxwhii.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qoxcbbsq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qrxlpqhz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3obbcoxvu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3pabpelxa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hqouwfop.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3uykjtojf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3yhrnblpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbdiqcpz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3acgztjmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewqnlaua.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3lpugmijl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3pzjfgdtt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fxlgugvk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cplfneke.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3occgqkdu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3djgqtdhv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cdccfgcr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3qohfnvhb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cckylnwl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uhjptvgw.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zkqsjojf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bxtbzumo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3csjuoluo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rtfilapn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3qaaiwhgq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ihvmewuk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bpjoaice.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vwfbjbof.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3cfjvubig.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3cwhwzsun.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vcjpjsib.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ejtmfhnh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3quhfsrrk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bygjyttu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wbdakdin.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ggrqqhne.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3uhbmgmvj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dpwtznao.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jtkegmxh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fjxcwzmo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3gsaksftk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bsalvrgc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vvnfofct.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xryhovov.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3slxbnghw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3monlkuri.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vxixqfbi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ztvupbgq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3affednes.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jsjcrelb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3yyuakorp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eewbgoyw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3uehlvdwl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3meewjixm.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ohxwwzqq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ewycykpz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mrnyhjws.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zlczzegy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rphpgjub.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3mzuxgksn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rtgyhyhh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tpdimrdk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3nwjnhvem.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3badubvhs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3lksqgqow.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xxhoaukt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3wnqtvlbk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3erkfhbtx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3hpqqwnjk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rwwfzwig.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rsxjaomh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3fvzleddk.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cdqzptis.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kztdzxdi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ivgkyqka.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3noidivgy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yybgvdzt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ctxjeyhs.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hryvsawg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcymzivc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tbzwjhos.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lwivswon.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ttwdevtm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3hseiofeu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sqjnwyjv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wayvohqj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qiosvzkb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xzvhwbkt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wsomwaio.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3acexbbon.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3zujpvmoj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wwykbpyv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sqykdzjs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3mtrmueht.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3plyuhifl.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3adqgylou.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ykxzwshq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3icekhfdw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3moydldgk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xrmveehs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zsuvfuct.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dfygjyhz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3thjuoztc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hcrmthad.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3rmzyodov.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3imhgfedd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tdnndltv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vjbdvqcj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3fvapynez.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mhbxsgcj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qtdvohns.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3hlvaknmb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3klmnxmyl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hmxrfdey.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vlumnhqi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ypvxuluk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zpmoyhvx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nzffvbiq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bekxpoib.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ernyeijw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hsrikdob.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3dtrgvehb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ksxanrxs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kcivtzig.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3zouoafop.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3iywqwmwy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3faojdorb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bxannobv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3uiftxtll.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ivuhphzu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3sjxvrmuv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pnhlcvqr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3eotvqdle.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kchkqgof.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cwetdirh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ldztkzgz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3wxxypwtp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ucbtpynt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tcmnxavc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ahztkjdv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3kqxtsthl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3szvltaug.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3odxuhqsk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iwprjilw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3tmxrujly.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oxbrvnfu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xawstifo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aqlicvmf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3wilvtinw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dgsztxxj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xalpdzpx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wvipleqt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3avbuykfh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3lcugrjsg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wafvjdtf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3tvbxjmon.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3enbgcyqy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ojtxcqsi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3umsmppbn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mvxmcctz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3qdzxslur.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3njtxoafc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3fyzemibc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3crtjevhw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ehmiziul.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3stcefjkp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3czbqwpkx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zheltpnu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fczxgqui.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3udivtepc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fmwqhjxu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dpllczod.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vhihdwmq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3bgfcaqfu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3iihkmxat.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jbmywxux.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jprbuwuq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jgpxsksd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3fdefeabr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3drsfdcem.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pqkbfoao.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3agtxbyfd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nclvoctw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wtciefia.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3oqmepxac.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3iwlddyts.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qzceyjvj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ydozrqrz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3sjzxplni.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3djrlxdlt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wkyivvnr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ekryfrlc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwojzjdp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qhaixkco.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zzibnzka.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dsicwyhn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgxynnvd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bxgjcyoc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovbbkbkp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nlquvmzc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xgqjloom.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rpvuqyzv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3sgjyousx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3urxexdzl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3gadcexly.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ppncsfxd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fnxukfkm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3lidpcfbz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dijanhiz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ksiyaqmi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jjenynbw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ednrnndx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zlzeuuqs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3gzhlxsdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3konojbuv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3sdvlbdou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srowlngf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3cjoyugmq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qbosrbqp.html


<!-- 参考信息 -->