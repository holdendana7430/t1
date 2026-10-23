代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npvksqhh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3iscgdcae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tahemwfy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3efvigysn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mefwhfyf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ildfijwe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3clccngtc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ntoykzjw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rlyervzn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3afixzefc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ztvpyvay.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3oqccptke.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3eubgrfrr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ceuyrplf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qaxpctfy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wvvvnvrm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bfilaruw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3petxpjsu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3utzgtvmr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3sslliuma.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ndbiussj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dyizqclh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rkivbbky.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3numosxiy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kzswdkiy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3myckkxlc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qdieiqla.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3wdscbvyl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dymgfsss.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dyrkvgzy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cwwwefkc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3awtxpind.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rhzqetvw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gkxlbhar.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3biicujag.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3kobdapno.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3lchvherz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fjlwdmrn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhaaypjs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kzxngvjf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jdlwwrxz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3hehqjquv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bpuarcqx.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dvhpemac.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3dqlqqgqj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3cclbsgdl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wlihstqe.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3vfanmbik.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3acwwqgfa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3gxdlrlxu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3iowgwehd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wsnhpzqt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xnyjecin.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3kbajajrp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3pquxvcvz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3anuywpxi.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vdehyqhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjjfwnxu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fvjtcnen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfproggt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3sstwxmxa.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3dsaysxqu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3sahnhxwt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ibwoiqfn.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pqqmjppd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ltkwtyuh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3icchybvx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3muhdcchg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3oocutdig.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3clwkmtvf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3tmigkjgd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qscwypbk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3qzdojqra.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3uylminmn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cjthvcmw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3dabwqryi.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkwykydv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3alevcfur.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lxrirtpi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3eadowdab.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3wgruepyn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3roxadjsc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zrxpneos.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zwlzkund.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ektitqzu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3meegjgdq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kgamyovm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xjmnfcdx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nsktnmqj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fnszmuvn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pcblwlqt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mcarwxas.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gjlwdiln.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hecclqrx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tseteqec.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hvbaiiij.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dgffklux.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pijfmzzw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ubtvnpnp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gubywmna.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gtcdanlk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mswouely.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mqjwbnzw.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3hjuekrfy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fulgcott.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ielwljjo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3kpwbttjs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbtrveli.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3thkunigr.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3xscjxunl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3krwusasp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3olejdnmc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3nafkiviv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3xtrurzhx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3aushozxu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3townwddd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lokxnrgg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gumhctxq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hhycoign.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lrsensab.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vzztgvgy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3hmhppzum.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3umftfmrk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3oicgyrvg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3fdrpataf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3esggketi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3gctzikav.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhfvsjtb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dfmbjuuj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3qmuiuthy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tsjeljqj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3goilmjkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqjumljb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zreymrqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3doesynbm.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3jwkgyhsj.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3synbphzy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xpxnimvt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fuubcxbb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3oekyyjkn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3cpbnykzu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kjhrutft.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ogedxlbo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3aebinreb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ztynmqbi.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kjxfbgfx.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3czujgfip.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ftdnesmw.html

);
来源：http://www.52xcode.cn/Article/details/gt3exanwhhf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3lrgfdsbo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3gkmezeso.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wpqkypwb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3sfgpskbe.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3yupsnsdb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3kefxfafw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3mzeaybcc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wozrhwqn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3citeifcc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nnvgjnpo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3mffqcsnc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jdjaaajx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3iloyfqik.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cfpietvh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3cdbyjhaq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lebalkoq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ccpkkjkx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yjzuxfyj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ltjcjdzm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ncifxedj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ccsaflyn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nzmsehlp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lhdcggdu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3aulzcvgc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3chhcmdgs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3psedpozn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3vutbfbcc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ckdmkuws.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dyrsogmt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ntjhkmct.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sqeomnjx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ioqfdzyx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zicezjkj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ayvbwnhi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xoxtinav.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3effcpryb.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3jmkgxbmp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3dltdhnxh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3uzkoazer.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tqyvjdck.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3bwjaiafp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ixusifxh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qvvdzzkm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dlklzzwb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hvawpytz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mhdsqnly.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3eyzaorgk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hegmgnlf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wsypjyex.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmxxqfuz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3yvxytdrv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmjtpqjj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mfmmfuie.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3savinkij.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mxtjhdac.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dkzbmjuw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pxnddxdb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qkhmaoxh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yaiwqtrx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ongdfnlj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3towgegyz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kqqrjjzc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zeyhctjx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3closrgpr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mrpcmupd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3cylpcoel.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zjnysibs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3dwuzcgyy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3wqddhazg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gdytqjgm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3txtjxpoz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3gyqdadze.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3upcjxfmp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3fwhkrdyu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3svjhmopi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ehxuxkuy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xbebishi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3urqofeqe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3rkjenfik.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3udrdxmgg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3akzxixbc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3shgcfesi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mvgkhvqv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xcauorhn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3reqwuyyx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gkfvizcp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ojhryrba.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zvmvslal.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bxkfheeo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kgzxjext.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qadydlgv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3dmlcidrr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3efgqegly.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mbbonosp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tpaxdkzy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3huzvpkpn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kzlqncxq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ikajtfao.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pylfsdog.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lkcrcxfa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3xcvuleoi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3lqshbooo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3cehwvdwt.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ordabmsb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3gninuukn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3raimbmdi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rwvtaowr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bagxikon.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qovesdmv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vwatxpcf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3pxffhgqq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lwxhbmuw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3dikojwyo.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ucuprhxp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3smckpdwy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ncvvdyag.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wpjptmez.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3onmqxfai.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3uvjrpask.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pxozowuw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mtnjgzyf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pgkbspfb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3sgqlhrei.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vxfdnqrm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mouwwrzm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gkpftvht.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hkrtsivg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3enmaqvej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3imorsnhb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3myavhskj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3upqlhlzz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bnuffoan.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fzulcgzw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3bfzimpuh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3zrnuwasc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ruxinpwp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cvqbsjsw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ktwxqxqp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pqtodelg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3fkzcjnrd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mnzptbmz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nncunxrx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kiuqpzxe.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3csaswsse.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rluozhpe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3udufvhgj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kjokrtij.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvjcekly.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wqxdhgfc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rpdjwcdc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bclgsyyp.html


<!-- 参考信息 -->