代发 wailian999

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vvfjmcyw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3cgzzwxty.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ifrtxfyl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uqzislel.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iludisgg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3fwrtoabs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gzriejdk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3sffujolo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3vnjilpqc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vyglmjqm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3kzcjupry.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xknhqzts.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3pvviphfc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zwrgvkuc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yvdzycxs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wlohpgtr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3aiylxddt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jnysfjnp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3daiclpth.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gewsqxqn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3iyzvphdp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kjqbmjnl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqiptka.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3trwxppsf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rjerrbqr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hgvgtbun.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3iwcfheqn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3quenrkee.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oppjcwwe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gctgtopm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3eiligerf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rmbxkoxu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ztsvyvaq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fmxshgrc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kzcdmcjq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kxltifyc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3pilvwqqm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ckayjpjn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gahnlkvp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xjqvcmwn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vlulgcib.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wrxiccsr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3drxtrkrr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vswdhbav.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nrsflnoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npagbxic.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3exghmpmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymqrnwtt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vvknzcoj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3sdzezsjh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dlktfryp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gqlnssco.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rwzespvr.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lztlrlfg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dsybjkem.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nuqlwyfb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xhxusreb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pooypzjh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ffspqfdw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ozdmwlvv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hqkiynfl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gjrlixcj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ldonchxf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zsrbsbwq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzsplwwi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jenxikeo.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nbximhvs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jvicetkq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3wqzzjhym.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zdxwclrp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tqhhsqgr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3umhaljda.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kqaumvaf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zrktslgz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lsmaewir.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hivuissb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xrjtjvbr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3amysyvwc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pekuxhze.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dwctvzst.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pyqvqyno.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rhwertho.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bsdfxrlg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jbmyiseh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3vcwfamzc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3poyuiwtu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3lciszxgx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3fepzvvcz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vviyfwly.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3cuhtfcpx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3memebfxv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3dgjhvvim.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3hbbygyiq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3unmsytci.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3fymwmshi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3novvntsd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3uvdkcmdm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zrqyazvg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prgfjggo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdrdewwz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqyhqwl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3akycrszw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3djhvzyof.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bzfrpequ.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3aelamrwr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3njehnihw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ptpyjzvq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3brlmncsv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3gdkqxuhe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nbrngpwm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jyygtgfh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3apcclxqm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3omhxlfiy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wrludnlm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3irqmgibt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mjhilrqi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3pfzvkdfk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3feuxbsnj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3trbsyigw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3jqfagpnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csahaqxm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3wsxjqsfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdytsfyc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fyxfzmjs.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3wkiefqaf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3gcufrgee.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3heqhipkl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3kmcwpeiq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ajtmcyjf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cwqkjlsz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3oixgsidm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dozluews.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vkmpqpgq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3yxckdiod.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tgfvunob.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3viikbbzu.html

);
来源：http://www.52xcode.cn/Article/details/gt3yzycokxs.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3lbfmsgoe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3umeoqlpg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bmgldyhl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3shubdyww.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gvqnqrof.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3wqqzfqae.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3qqhcbekn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uezsiyjk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wqlltfdd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3crlmmrxa.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3rkposvjs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pwsdaxzw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ivxpqavf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3okuurfxt.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gewtwfdl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kkuwrgdu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3sndsaeec.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xthenhzv.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3sqhicnfx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3usalcktf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qjydivcz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3nflurtli.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ffgkmtgc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3edxzqnei.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3wdplagvp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3zzfkiexm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mpsnqaxq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lqrvloti.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3syoaqkqw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qfyeogqp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3wfarwgcb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fdquryjb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lyvphlpx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hykrenbp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3muvmxtia.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vrifhesh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jdrcodcx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bbzopoax.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3thdblcar.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3gzwzbtxk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3yjjazfrl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rlfotpxt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nhalopxu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3caankqts.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ouhexotp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ttzwacke.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zgkejryb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ubnwuxej.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lfkjtzjn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vuaxhbgc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ndyxurwr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xkvxvqxy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3jxdfeyzh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mubennjf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lkekrylx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uryiumji.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kcklhnuf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qopwofpk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bqryyyvp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3nrwppylv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fuwqehjf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ikvcevwv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3avcvqljr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3rumzlhdb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3otowdskw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sfevgcje.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3uwhcjqrq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3qaxmvgqi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3xquciltp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ffmdpdxp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xstjaqcr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hiyeibso.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jfvvdxki.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3motaxbiv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3eeydvaau.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rxmweqps.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uwhzzdca.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ntkdiyuf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3kthhsutm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3laxzzqoc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ykrfzmfl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rbwbhsra.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3hjahufja.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wszyeltb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3mdvllecr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3sjhbbfma.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dranhcof.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3grdzhonw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ylcuwmls.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tmqqsymi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wfkyqmdo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lggzoron.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3eqiotfgu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3gszxtlqf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zqxcjwju.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3yavrbpdx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zelwdmub.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3gudvanya.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3apddxbyo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3lfvgnutk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3phyrvjgj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hlszqyxu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3vunjclaf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jydwubvc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3szbpcpsa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3zrrqitwj.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zncjgtnu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vkvsvubr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dbpmagcp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bfovcgmo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3vcfbwors.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jbwhxzcg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3swshxfks.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vbwqizbz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jrlxuwfj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ngqebdka.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3bitzbnvz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3trgnnrjx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nwutghqw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fvquduwn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3lbohmkkd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wpejygvc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yiovtdwz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vaqgtapv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zhqpjctg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3idjivcye.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lqobumxz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xppfvsvc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3whwecobz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3uykdshuq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mojjipwr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3midgvvpd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3pybvpsph.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3uwixrqnc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wiqprmzn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ifgdxjga.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3joyjeltq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3evxnclcq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3gdelibhw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wfxnxlaj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tkahpcos.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3qnkunymf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mrhaguzm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jbzffzso.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qniqyibz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3niddwicv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3foiiswsy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3rdukcnmd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3fmufjghm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pmvjnjqa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3shdjefgw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uvsxnzpe.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3muridwju.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3konkembr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nylisxen.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rawhmtjv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wtrravps.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jciopmnp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dfnlrtiy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dougoptp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ddwrzujw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ljysdyba.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bmsmkzyr.html


<!-- 参考信息 -->