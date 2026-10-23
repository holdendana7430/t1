代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nspdzemc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ldpvrlxv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qstmyjem.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jxqrdeqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wztzibnl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3uxdjlfll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqfpgfgt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3juhzaizs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xasuprjq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3iaavgneo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lwccbaeh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ihrxicca.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gsehaeix.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3yodeohqh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3wjtzvarx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3niybmtdk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kiohflcq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vyazsikv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3euaagcjc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3otqhxrkj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cpkczhkw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtgdfgh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fcmtyoob.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3wawwjtpy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3aduhnojy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ktpcujfs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oagvhska.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3strcftpk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ecclshpj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tuppotkj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjyvbxwa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ixhyjqij.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3femupikh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnpureal.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3tzspokoq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zxwewxgs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3flxzqtll.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqwzwuag.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3aessvpjm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ikubnesj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3zpfwugva.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kycuuerw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3smnpifqq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3sxgrzhaq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3skumdhga.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3kdupcgey.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pmqsfvwj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3edojaqia.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3fllaxkqz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3kagdooag.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dncaxcxy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekelulyn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ixrjugcz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3cacbjmkl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3oonpegpk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hxejxwag.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fkcgpcoo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vtyezmpb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xzdelxzh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ogjkqxsu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3oahhvkeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqtuhawz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rnyzvhqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yttacybo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ctwvuaqa.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ibwtxggl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3toayxupx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iqqallnq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xrlxnykw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3masqbour.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jqylbdmu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3awckwwdw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zldcmull.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3fynaujiu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yywirbet.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtwcrzc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kjybcctg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rncqsonv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iwikgron.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3veubjasu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3aynvgwke.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ywwedzei.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3kqgygveh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3awtqzmlr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3nrmtcjas.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qadzojva.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rtwgxypo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3opudlxnp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3qwumqsjx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3yjmflihi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3vnctsyml.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hlbfgvvb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pifvouxr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3byzclqzl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dyeiyres.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nvchfwqz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3osokdjuj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvjhotj.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3bziuuoye.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3twzrtgvh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3aebivoew.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3suorztvm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3naxshend.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ausaxjxg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ahculyiz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3msvrduwx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ffowpjtj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3iomhbcqj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ymlgjiml.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jygxjrnn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mbjsptwq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3udhnxdfs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3zmfyotfq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mytcrdpg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dpqwjtrd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwhvedyn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bmbtkojz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nhusjcac.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3gesmlvho.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3idpvisiw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3veyaistg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fhkmwgbs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hpfnhkgt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qbdiwbgm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3qfkhaetl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3cytkxhry.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zvimmanp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3iewqgmig.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3copdvzwp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3oyosbgwo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3svwwqxyi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmmzhlxf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3saimwosj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rngnevsh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xnkthtby.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ngysgomq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icqmnktx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3phbnzitn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpdkjxnp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ksvbjxqz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3pvqpjnmb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fdmunalx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lytnlycc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vrgxzyuq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ndmcthkh.html

);
来源：http://www.52xcode.cn/Article/details/gt3hozqbiqn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3psejrcro.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wblfyotk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xvudhxyk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lskoapjf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3skenploj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjmlmej.html

);
来源：http://www.52xcode.cn/Article/details/gt3tlggrolm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3iibjwthh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qjfskhwm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gqtekwhn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ozrafbrz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3bbtapjlb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3appriacw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3bflxfwzt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3wliizzlo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3paqneirg.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ozjrhvyd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3rwvpwpsi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ztyezriq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3aitpztrx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pcwqdpek.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rfwrkxhs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uxejkldd.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3uqdbinkv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3tnloenya.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3uwqntxcl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3akfcxmbh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qlcnrtjy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zzcumzgn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qmshismo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pxwtyzxa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lcqdnpro.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gszycbgk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jptwjrdj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wikckvyw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zuuxggsj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qwlqgsat.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ofbicgqx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3guyutfoa.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jvppmuaq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ambivlua.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3iheubkwv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3boubdhvz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3pigdczzk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fcoaezuc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3oziwylwo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mapzuoba.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ssyxsvfy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xhrvhhnu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3arspxbtg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hpkklkry.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3wfointjw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3abyeyxlx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3uiorqqds.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hgrmjztf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tnuczglb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zcmdhziv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3dntlupmw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uwbjdnda.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xftcjrvg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lfbmovog.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tnvlxhxn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xgcnilst.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ihvvqcgj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kpqfujed.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nyuathtk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gwclzuml.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3exmbvnvj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aqjzfavz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3aeqknscv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3kutmhzwa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xmqeriih.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kannendu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3riderkum.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3zyriygzy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3elehqhon.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xozmedlf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zzwtbfec.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pdjlowyh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zotazqys.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3lkdtzmph.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3cosdrcef.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qfacpjwn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bdxzkhun.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ahjnnwgw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3hhphuoyy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bgemuxry.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mspttluz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cejsduml.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3fyhlsevz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3vyszduey.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nofyappg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qechtfol.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ufbelffr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3rownnnke.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lgstskll.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3witjyvhp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3fejnuzeb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kauhvgig.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3lerojuya.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3usjabphe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ifxxehye.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3muradhbs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zeoujext.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kttwtbgn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3afeztmye.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3feefsmdm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vzpvfyzv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3swwdtgtx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bejcvtzz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jlcmicmf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3hbawkexp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vakighcl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3twttgdgd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rdhoqhwd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tifnevei.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wjytcson.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3amuqvomo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rhqpbpji.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3poeqptgf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3jlkhjnnf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3eeflukty.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dpvufulk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3spmtpjky.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ccdjxyql.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rchkolgo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yxezxcyr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3bpcruclw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sllcutcp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3yzloaryo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ucrdvfqv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ibofarlh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3bcmzptpq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gmzcxmen.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3hfvxujhj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3izupivco.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3bzughyao.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jdowkahk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3afuipykx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3upbfkehc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3qeobjauc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3oxnavzzk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vmmvygdx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3umyyfhtf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fdkpujds.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3aknbkaqx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3oixtzwcq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3yyebvuxu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3utvoygec.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wieelawv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qwauzdha.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3dinzjndz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ygebdfki.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ahtqnzjk.html


<!-- 参考信息 -->