代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fbqhkjiz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3osbilbzx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pwkarwvg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fbqhhibo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3eixvkgiq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3egtmimlw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3djqrlgnl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3vgpqvinp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3iakiihez.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ilnugaog.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3qxqcyfui.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mpfcixan.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3onsjvvcn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3izpsfpfg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3kqnkocku.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3toprkvjq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3jwzmwjjx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3azvaktut.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gvhrwyte.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3dpdjeqcb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ymhdbqzi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wtwbesaz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lgiocmzd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3itrkjqgr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ukjfpobp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3laqywfoh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3trbhpdqn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tlfvfhyj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rctumdif.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3burkbdta.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tidqfldm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wtuolnzx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3byplcsnn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rwmzwclz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwgonowg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3winwexgb.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xzcffgrw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ezviryfq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3somlcjlm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3relddqpr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ketqplaz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3udnibfpl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qeutuuwd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vweooski.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3iygxecva.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xqytwgaw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3clmbtbld.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3imcdbpcm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3orldogic.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3lpqvmusq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jzcnwcyx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3inaihyfm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3uzsciaky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwfyfglp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cytsqpjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezhuiihr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bqaotwpb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qxhuplvv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wrmribnv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kgwfzekg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ypkauihp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lvgegmgk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qsekuyfm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gzrczbxn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3esntmljx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3soerfhvf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3sdqqltyi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tzxcfjcx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ttypwgdf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3yyysqntq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tuvhuqzt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gwkhqbef.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpduyshb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3piwcccnv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3soyhyvxu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3sintpkup.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3yvialner.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3boxldncl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3exycgbeg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3cobggawu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zfybseae.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3urmtvpqn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3pjieqjuo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zfuaaaht.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3oddaahtk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zuirikta.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wjczzgnf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zokidwuk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ucqinyxu.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3hptebemi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3hdxukjle.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fgrnnfmc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hamxziwr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3iyzwlgyo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jxshssqa.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oiewqkcj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xnjoewgf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3yfapansa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3puumfdjc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qkapcyvj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3veqcvdnw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dvmusiml.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3yqyjktcd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yrhujdlb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3getzxaay.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ywjwkkzw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qwfhkjjs.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmzuoerw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3whjrfjod.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3goyiluyg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lhqkkwdu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tlabdvmf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3rkaeupoa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jlpklmji.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vyafzgcc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hyhamenb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xqukehfa.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kreesfpv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vixadrsh.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3uzgnmhpk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3leybvoih.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wbbvnvep.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3sintaqim.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hynixzxh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rachvtgg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3lbbdsadr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jgolxyoy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3etugbnhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmytctam.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ailuxiii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soyqjojv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3yaepzcrf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3proihxcy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zjsxzvyf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fyajqfhi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3hbwslgwq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ismyymty.html

);
来源：http://www.52xcode.cn/Article/details/gt3qpfiedxt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3kcphwuti.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3yptksizp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qjcspugu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pzzxjcrl.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ehpybquc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fosgsxmg.html

);
来源：http://www.52xcode.cn/Article/details/gt3chqdfjpl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3wmurepqk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pjgqggcw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3gxrmiost.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hxbchnuw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hpjvdvzz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yfihkteb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fbcfdcmy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3leupqtek.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ilkytdyo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3oaylelpd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xwsmrmgv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gxtwrsdn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3bouldejr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ivzfircc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3eihiopvg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3scodqgdi.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3nfoehecx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nokroafw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3yktnsblc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3pueminhi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vhipstry.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3nmxdjspb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xraohrbg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3zvtbzvdp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3woibxjtz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3czgypaiy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3gzhwpeys.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3faowtzba.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3lakkpaia.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xhkhjndv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3agucphnh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xbzlpyqn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3uzidxlkx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zrncsqlp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wajzchcl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hykgdwhr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jcphaclf.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xdzwurtt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3eacvweyg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3uhalucfc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3okumgboz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hceaeepr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tyvfrvub.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wubjnemg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3acvraowm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfurqorx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mnvsmxwq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dyhegiks.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qjoutzxn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmolgxqw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3nxfyttng.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dozpticf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3zxjrsdox.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3daijhaba.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3silxrina.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmrdsbjx.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3uukfpwjn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rlfvddvv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3tpeujehv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mxmjcrxc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zwjdlnsg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rsqlrjtx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3nygcjosw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3mhnlzrqz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3svkokqfk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3rnywgqse.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xqcwezyu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3nhznxxkn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3xrrgoils.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ytaimfqo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oalabqxm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lpcsxesl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jvgfpafd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ligmkiyb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rzyopggz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kwupgauq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ssgjcozu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3uydwuuti.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wwctncmq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3slvemzww.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ppcazurn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vhqbuzpa.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3iggjyndd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cnmnittl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wctizwpu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3luycdoyj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bcnkinxi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wxzwjbzr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zoywtuaw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3dcgfmbgs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3rsdpfgbn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xfvrreav.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3duarlujn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pnzumcjs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dkfuivls.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3afvgypaz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tswvleuq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3parsytko.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vijozahj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xzmdrvqv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3axogxeqw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zgwsgwdk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lxsocvuc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tylofkyh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3nkpyyotn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3eocpwcit.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3sltflpws.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hvcyxhzn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3gkksxcwc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wzqvsjit.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3efzhfqrj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qgujasph.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jbhklfes.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dpbffonl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xozndput.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3slweshrc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jqzvueom.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lpjbbvaq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3reccgfwr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rldmkxcb.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3derrmrev.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qlkfzjtz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zauoxvnr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ljgsohso.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wefhrhjt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3neftxbel.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3scojiymq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3pcieyuze.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oupwbkat.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yvojruqi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kafyshno.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wwunsepr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3bpxnidex.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lmxbazsr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mhmzeauf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3chdaoovx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fzrwgqms.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bfrawebe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ywytpgwc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3lmltxvgf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dsdwkkye.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dfaljohv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gwdqdvty.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3dfhvkcdz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3aigzekgv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ctuxmybp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3fefgslbx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3foxqrett.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3witbpevm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3utbdfkqo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wnqdgzji.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jghvgnxh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qllrgryw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dllpcmrw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xwdjuwss.html


<!-- 参考信息 -->