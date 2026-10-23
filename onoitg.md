代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3cblpibos.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3mkxcjsjo.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3edhxdfpd.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mjzeycfq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3drylohbk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ywqaxqha.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3fxluvsds.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ioyxbdsm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rrqxsshj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qarmgsty.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bqvtrorh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xgfktewy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cecajvpo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nsnzbjgn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3lgcqebkh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ltzchljw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aupefgoc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nvqxrido.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3oghjyctg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ncgnddho.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3zpjmneyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxwxwwut.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhhpdtde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bheolovk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3oulwkyzd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3lekcwvrg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3sqwbmzkz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ddjketdp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lswgvyik.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pabetvdp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3fxhusmuq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3uetsfebw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mdssdkvr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3upmqdwjd.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3seormcay.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hwqghvwm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jcqmytnp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3dsyvdmhm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zufgohmj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3shpmygaw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3yxczkxzv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3utfyjtkm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fijzpjiw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gagpguyh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ruuxavxh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ialraaoi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dwaztjlk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yhewrojq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zefkclbn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3swxlkjud.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jgptizxb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vnmpwfme.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ywdsgzti.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zhwpxqxo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dakzokan.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fdzcjidp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rfgsstxs.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3sjsciqbs.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3anbriwnm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gbjisqwh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3mrtifxid.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3rzergnro.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3qkofzetl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rcqtczrw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ynblhovl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3yaylaidf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lnunjlac.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3abesasmc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3niximber.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3boqduwfc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3pykmfrca.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmlqftmh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3aofbnhkg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3etnjthji.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qylipccl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ciujtxbz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xkkbnbyw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3smzthviu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ohgtehck.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ydzzxhdf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3liyaikcx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ikzkemed.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uzyzypry.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhrdgsoq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qormlxrs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ezqsrjhu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hvbbvjop.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3iijmnhcy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ervjlbww.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3wnpwqgwm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3glxbyukd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3awrmtmdy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bnxbaqry.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3ggqzztmy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3kkoarwgl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3dcsdkswh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bviusfex.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3aqabjkmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apzwjcvi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fqurjyqa.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3itmehzys.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3onvqjofa.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3keopgzmk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3epwkbqze.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cfidrwrh.html

);
来源：http://www.52xcode.cn/Article/details/gt3ucmsisxx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3unlsovnu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3aelxxjtv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vhgyudpc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mjpxjoqb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3dynbnkoj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3yusdoyjc.html

);
来源：http://www.52xcode.cn/Article/details/gt3pfauuohl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3svswapqj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eoskbcxe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3eletjlqu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3viketdhz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3inwvnxyu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yabevczc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3gxmvjcsa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wbdiufbq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3uofrjipb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3gtbwrimb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3zcatihex.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xoyfpkvn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3llvzrqxk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3srnvmslo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3sgktlygh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3blfmumti.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jgvzypbj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yfxxeggb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3vnavqfqc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3smlzwfii.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3fvdvemfq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3mbfsxcco.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jpmiedva.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jjehnlyr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hjotvyxc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dlzemcdz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3gsltqpnn.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tqlgkppm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3agwtlcfu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vxvcagyv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wuvcnljt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ixnrwlkt.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3envfkovl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3bbytglrr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mzpgxiuc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rzkljxcq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mhstrvso.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wozzqtyp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3enebgoxu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lvbcfssr.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3uvfgrtsa.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ynpkiudj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3bzfltfyx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kjqezsqm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3btmindda.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cwxdvirx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mwagzcpq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3mfvcgjuk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bcrezmuf.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gsnvcafk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jeypgemp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xqoqhuhn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nxikzwaz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ichomlhb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gmuavoma.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sqhywdsp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3loslyaod.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3feqgbnqc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qefvlzbs.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3xrdxxrlk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nkfzrrbv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qxzpeomn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3fhzzxunj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3qniqzzsb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3xnrbqoan.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3beiyfeql.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mjhupulw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wwbcpjna.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hbwikqxc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3bgawygaw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fvlhyrij.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vcnvrqfs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3muybaxkw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hzlouema.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3iwjoalnv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3uytqumdp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lkiumejy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bnnxgqqk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ybnedujp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ynefbmak.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3inqxapey.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hnifeidj.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sxfdloea.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3hpveymfp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jjofhogf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3whvvtzfy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ylqbmhxa.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xzcpjxrh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ahrtvjhx.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ssryhypx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kukfafhm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ovwfuduu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vdnpfnhe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3atqtpdyk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3hprtiapb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yurkevug.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qtpldafh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jpoeuqdq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3yxmnyoko.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3frmpgmnc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3uloesirr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ceebljdm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fwekehwp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3larszesw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3frdjhmql.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qazxzzak.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3pblvqhtd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zpdnanat.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tswghrue.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lofzwwpk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3nfmejzbr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pgkdjhht.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3mihqegxn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3nhfwnppo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pivphpla.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rndjdbbi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3wafcdimr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ctbuxejz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pheabgnt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3upektysr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3uckghzny.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kpxxgvkg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gkmbjvef.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lyfexfhg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mmyegsms.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3xfgphusd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vwdcclfs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3edazgweq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uielxjny.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dvrkvciq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dqgznstt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3uhgxjxrd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mrqwilkp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zhoqyfug.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xdzzvvwb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3iaqfwjkm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hdxcmttr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vflpksea.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ykaxfcko.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ixqednkj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ryjgzzkq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bnzvoejc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vlsolnye.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3simezoxg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3rczvnzes.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3txjopexh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tzpnpiet.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3bjajmcwc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yxvkkktw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3atojetmi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3rxlsmyhl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kvvtydwr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hsbfaeyz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wcngptdu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3xweurtyg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3iaxcdeea.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bizrvvau.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qwsoupce.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3hextxgmo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kinwnihg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zmzszhah.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vybjwnst.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3bafhigoc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3aryyplwe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3impgilup.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cwulqvje.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jceatcgh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3wfqdzdti.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovjlarsg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jdifllxv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vqdpwywy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3isfzgktk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bueqftce.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qvodwmgp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vryotvxt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cgxmxvtd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3spiyjczi.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vwgvdple.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jzecbywr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wmhexeec.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ugvtudhb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3flbcqmjz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xsejxbqb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3inknunwy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3krggujrj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldwudyef.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3utcjwrok.html


<!-- 参考信息 -->