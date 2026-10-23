代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ebawaqwm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlmlbouq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zaajbkty.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3szncysck.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3etoyjkyj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3uwqgiptm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jfweowrq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3iybrjuzx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3majoycyb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3yjjyllev.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kpvsfozh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3xugbehjs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3erifxrkk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rzvchnnb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tymggkzu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsykyna.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3lidgbzzr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zhfdoxzr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zcvrvnfa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wysvmioh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3onrkvlju.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ikueconf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3vgnkidvg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3egswsikh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nndyjrwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kriiyimx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3egbzunwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nogzirae.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xjdhlzxp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dncalubj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xyiptjgb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nedcjgap.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kqtmjxxf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3alnodzzt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vyymfsmx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jcfqkddu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3smgocugf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3gfufobgz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ikonspox.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qtelrutt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rehbjaco.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3aquhzskg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3imodaxks.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mtcnfqnj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3yttponyk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cczixobx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3emymnqsk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3bsnofghx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jmqoilkg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fpgosfdh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dfeisqrp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wohizbln.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zfepyhrq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qexjvlzb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3bytdwcxq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qeilpqys.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gikdocmy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3axfxqoyp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3qajimoql.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ebbcumbq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mrlsdphs.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nrfpqzwh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3sifspbpt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eraddoij.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3qawycucr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rttxmbfe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3sehbivuy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qyiagdou.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qlvrvhcn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3cwcpnwly.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jvuquczk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nscudtxt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vgjmqdlv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fxrseaqc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ipnsmgxn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhoggyfz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xqwefpcl.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mwbpuhhx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pegjoyxg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ghjcwjuf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3fmpdnqpt.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3danxonbx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wfvktdxf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3nnuqpanl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3rpmqvcnu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kshxippl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jjtlacaw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3subpymio.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3iszxchnu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3absngyst.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3wukasmts.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3cwbbtlma.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3pwssssyv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3rbrnglfh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3orehjdpj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3swktomfj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mukvxtbb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3trxrvrls.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3dmbisyqp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3vflbyzhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3farggcxt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cazbofoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dexxvcte.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vlmxlxpf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qauujvhy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qaxuuodn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rxfabaox.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3puzhxjwc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3gjlomche.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zixpdnnj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3clsbwjuj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3txtajfpr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bsptgogg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3obzwytrf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3gfvroytq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pyiozwna.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gchszmgd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3zscymnqn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ktpvuncf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3rcgultqx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3wzrxglnh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jslqkwmp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ueuwvakk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3otbkraxp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3wqtrwubl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3dhatoqvm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fglolfvj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3waxveqme.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yoesnmsd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mrqoniuh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jqgcidzi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jiznhxpz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kbxhfmks.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pvjphdkk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mgiublyf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3nmltfcvu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3cjvwrddt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qlhhvpmj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gyjcctvi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ymieuysw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3egjuckuz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3plukqfjg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fdxkuoxi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3budeylxt.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lapoockx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3catzfapm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3senfffxu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3nqdyxnes.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3atpmfslf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ddyhqjba.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jtxfsrml.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3radhxqup.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3edmqqikt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ukyoaylo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3panndhqt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3lukpyylm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3roysjaqh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qrhqrdza.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ddrfukjq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3aqrmsvmk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ikwrbtrr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tlkliywd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfcstdft.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mrmpktjx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3otxgutkf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3efcwbnrv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3devkwnup.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3nxruqfme.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bwyuvjif.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3unlytbuk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ijaarnkj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gekjvvfw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3toqvgrxt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3mfgwtufx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tegdgazl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3csbthoxx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3knwrxwkl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sczhboiv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uztyfvsa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pyiwddrq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yiiznpvq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3uakescrs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tznhotqx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3kocnejnp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3psfgjryz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yoknqnbq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3icbwlrxt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rnvanpsv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3rqhewbwu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vsqjjtai.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ptjtsmct.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rzoacnsz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kztyofim.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qclvnkck.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3eiktxrtd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nfmzffjc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ajpqjohw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jwtbqoxu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kwuwovwo.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qavhqaoy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bvexcaxk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ejzwdjay.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ilivjuxj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iqkgsyyy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3lqmaqarn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bvqxwqdw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3sgbcqyca.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pvfvvpiv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3uxddmahn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rxytgvvt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fgpjmbru.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fprlxcxb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3webtaisa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3jbsxqway.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3emygtitq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ttojkekd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nveemyty.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3daykvpcl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gvasqfhn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ntzzalwi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uzagsbyw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3amvdhyuk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3inqcwenh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zonfyqdi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3qkaormvn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3rbfxdcgz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qwqmydeo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3itzssutl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qrsumdvq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3dplpfyua.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nqzahjqe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xbwjwcsd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3txoyllqp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3apnaiqsc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3otxphhvg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pmrktpyq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aunzclhl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fjavbmem.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3itehjjvk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ajsibsps.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dbgudinm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jrdfgroo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3udxqtzlp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qafbdimq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3jeeweuyi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nfxomzus.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zabsaivy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kqqjzcow.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wwwgvesj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3hvsiqhow.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3efnzfrak.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3bejxewwd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3antbxgos.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ihknylli.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3cbmgicog.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kuexiznf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3sgqxvuxq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3txkngaia.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3sylxksfu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nzicqytu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3brclsvbt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hkfzewfm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3isgyxugm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bggvcqmz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nunveaxv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kxnwuxbd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3mjwmgxtu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3txfxiyxt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tyahcpwb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qnetkuaf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tncfdhus.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uphzbtry.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hzetruga.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vlyncslg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3shfzfqgl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qlollyry.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ssiscffx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3mscgicit.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3szaerudo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3sozplxdp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jtknqlvc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zufvejjc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zdyxfoar.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3vufzndjm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3lgprgnmi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ynzmcfol.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3boqpxull.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yshtvcnt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vvqsqzso.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sxxnesxz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xyrdorlw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3etmfsxhu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3iulzyojh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rbjydajc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ovshvsxm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wpuoznvb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3radimkcw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3sdsntyir.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ihckajrb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yerueqhe.html


<!-- 参考信息 -->