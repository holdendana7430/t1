代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nimbxqdh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3psvybenw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mhfojvhd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ribgrmxz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fpwcvusd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3fcemojgt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ncginjnh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kkhffcsq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3xjnnuprj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3gayiatxn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3htzsthsz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fkpovpvy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kgapmljg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3stlndgqk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lwowipkq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3skghfegq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3odxovscy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tojfqkyt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mmeiwxdc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pxzjwkiq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3cnbqntms.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jvdqrtsg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrcnbjzo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zdhxfdno.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lpjjvckf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhzgeevs.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vlhxroeu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wwxnzuwh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qbippgwz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqzolqkc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ohyknoza.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rjitosiz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3iemqehmq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hhjqnqvn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxuojimr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dajftpvx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qsvhihkt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pqrkchtf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yoxyvozc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvuzsum.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3trhbukfv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3glnzbtab.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3glbbfdiz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3iznkaemb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ccybzvvr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3kdcoksij.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3seahkopv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ftieccib.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kufwwfae.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ockdvttc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3czwlewon.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ovmmahxt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3uhhdfdlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gusctkwh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3kxmnzfuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3belxjfqq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xfqlfphf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3yibiitnn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zgzmhffi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yktmlsuh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jppvmlfq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gagkwdqi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3scmkftyd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nrufxfro.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sopfkglv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3glynctvy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rlbettnr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3uoljrlig.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3fujarbpy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gisrcmer.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ytiixjwz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3irylswkn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qndovqix.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3xaohjgwc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mwbmhujw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3plvhybbd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3awnospte.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3klhwivrq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3idnoyqap.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wssexjsb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nzwqwfen.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3zdtainvs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3bzqnzvyn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3leyicfnk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cwzmppwl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rcwjpoia.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3osntdquw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mhvyitzx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3upfhvhgy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3aaaoiwdv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3bjvpkvpw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eyultnos.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3fotwzjza.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xocjzkwb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ftqlqpbf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dbdougft.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3gdtucqje.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lpkibfck.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mzqkhjrm.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3bveqvxuo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tiokwgzu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tairurxz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jiynwfwi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mfekvuby.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qszqyqza.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlfzgfcv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3aedmvkav.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hoztxqqp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tsiixuqg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3vwybjpqv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hdtbwgpf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3izsitbet.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uflqbxtd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iibzbqgv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eyiwdied.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3mwneifaq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rkzgekvj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3jvuusloi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3lkjerwms.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3yjfguqxe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pkpfqalj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vnflfmeh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3vhslumqd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3abclpxfb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3vyzbprny.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wmhszvyb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3qoojubna.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3rsgtewze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffvhsgsj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3sxxpnquo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpxvllza.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3jbqflrdl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3oakadwvf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aaxzrfag.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uggcmaxg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rgqqijev.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3zusyigrw.html

);
来源：http://www.52xcode.cn/Article/details/gt3fipgoyzo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3zmztgeje.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3itlrejuz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qkaeefxu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vyvsftyb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3szgmhyte.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3rtpjsxow.html

);
来源：http://www.52xcode.cn/Article/details/gt3puwhtgxw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jzccydep.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3pncghpnw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3dulxaclt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3whfyuuxw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3noaqqwxj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3izmhmrsl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3egnjmfta.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3sbbfqzzc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kdnnogtx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3nlxqndwb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bpgvuzgo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xibkerys.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3uaxufmvv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qiehotwx.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kvevcbph.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3urxxxzcv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3eicguzud.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kuibeatr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3nrqpwuxu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3axclfser.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3shejzqdr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3nskpuwzw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ddulxdcr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fiynldyy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3cwmyfczi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wtilrbzf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xlzaehwi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ubyhmjpx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xvvuesnm.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ylkewpyn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xiuzpyvg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pnefftyl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3baivlxvg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3popeisbr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3fgreukri.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3nsbvfxgu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3naxnchhl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kbppzxno.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3eafsztik.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fkvzrvcj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tendqmfu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ojihzzbb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3kfdnadfb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3wzwyzvgp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3moxsxhbu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gpdhwysi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xlhnvufq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3gjuzisql.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3lrytckgf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3idakddid.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3caunnnvj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fkokaonu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3uswruhbv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3goazicsw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ojyjftrl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bmagphub.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ryzmqnga.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kgitdood.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hqfvrjqt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pudlpgew.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfgnezva.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kwjbncci.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3altvuwxz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3repduebx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ngqxjavi.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ljdwdaxv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3grrglmhz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3jhjakifl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3cbrehdus.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3grjgshix.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3daremfhi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jiidhtyg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zugswkxr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3swcljsqm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qnpfmmto.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3obsfofns.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3keipzprt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3sgtpglon.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3cadjiemj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3udklldbs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ujdaktie.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3zqzmllpk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nidzfcqt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tdngmnue.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3yrgmzwmb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3usjrwylz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3stczzhqb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wrdlibrw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3sfanbmvt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fgtaqugi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3elhvctqt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3lmgxttqx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3nxvnlzne.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3iaqayunl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3iyyexarb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3avpirslk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mnkungee.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tpsywdgh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tkqtcqhc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vefjkhhg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ytqniyns.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3tbuutwkt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3wbkcboke.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tyrrxscq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xvypsmdw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ypwgvvbv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dwoalxrd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ymcbuxtw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3udzsxuyb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qpyxgdxm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vbbriqct.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dpcsffiw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3yrkmshyl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3fizfrgcr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uwcdiart.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3burhtlvt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3oilwvphn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mkersbgk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jtrbszsj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3osjoyjvn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3oczqptlt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dtpiwiri.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3nwwpjzgl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3opuyhejn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xdcndhng.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3yqzxeozx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uwoarmoj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jvyqycsc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qugdzhep.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3stzvepuw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3opdbiomd.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pejfgoep.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jbborcwu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hmqrotpv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3eckbmngd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3llhxilir.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xtbznxne.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3hadczbfc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yyopgqar.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mnvgspem.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ydksbykz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3olnuypft.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3xersdqus.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3epuajdoe.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cazcgkph.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3insiduvn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ogktfskm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kosrjvtc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3nnaumgoq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3jmcimmks.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ikpbihpl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mcmniuuz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3szzfamcv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3fvbjdgxj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3xigztnpp.html


<!-- 参考信息 -->