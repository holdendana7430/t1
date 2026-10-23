代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lmzjaufn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3opzoaieu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3fqlzmidk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3yawrqele.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ltoocfqt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3sxliyxpg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jzsvikgw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3auwrjqps.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dqtaypfd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3swesbnfg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ipbnpdub.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kitisemi.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mcuevlsl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xfuaulzr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ndidrchm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3fndazlyv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3yumuebtj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3loieuenj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tqihmqbs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3jzoqzrma.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pkdkisnz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3btajtjlm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gdzqsjdh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3xelblkni.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3romrmoqa.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhcdsegy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xstkttni.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ckypdlvy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vmswgmls.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3taxkrffb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuuqghnk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3bqlutzcv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3uiadrwyg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ividlwau.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gxlzphoi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dpsdyhhh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dnyrfngl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3svqkwims.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3osgdypdi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jzqcgtqt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rvecawzn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mjxmyvua.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mycrulri.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyixhxgr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3yjlnyqxb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dwyxeaec.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xfvugfsq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zxcubdje.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rxpexgyz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3lhlngmll.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3pzihexfq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zpvxraco.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3iabacyei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oalyevrf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3phprgfvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubpsmlcu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ovwxpiek.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3xtdwxoeo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3oqrhsokd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lrafgnwf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3icwjicrc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dumiyvys.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nmaekhxq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3miizfqgo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ltyayccy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3npciyfrn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xzuamgse.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3yvsrytoq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rrocfypc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gamlvfmj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qgvmqupj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3mmqujuff.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3dnwhzmdt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3jgrunnbx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fzzmzvfj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yhqwlcus.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zzllaequ.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bazxzhkn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vfbcrfeq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mpyhrlgq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3uykeasuw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nqkgohdq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tkgcmjry.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3lzvybkxj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xvhsjdun.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ehdxpdrn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3aaoyunwm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ceaxegry.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kneyqggg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3nysvidlm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wjmilvhc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qdkbreym.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cwclojzk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3seylpzmt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nhdmdvto.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xfdibxaj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zsprzgxh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3rzpfbgne.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tchzctuh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tvzxxzmj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3emvjgfoq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3oxldfcpz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bvjsxnre.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkbakxvi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3btpjstgn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3kzuxvaaz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ymdmtsbp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3uayklvbk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xkhxktux.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3fbsjoeil.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3cghqcgil.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lplerzln.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3fzzunjbb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ihqfspxm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rbcslzbx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3iqgjkgsg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3avhkibrk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3sjjqvqcf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qyfnuwrt.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3dyqmzxcz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3tlkptykb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ruwzirnx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zwubiqwg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bafcyrym.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3gpqillny.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3phesgfgk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kurzdnic.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3uekvvper.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plesxlag.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3itmeivtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjurxqvw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gjzfnamw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3yqefhzgn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3cjrulpuq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yeymwgnn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ayrazmqw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3wuijybrc.html

);
来源：http://www.52xcode.cn/Article/details/gt3tpkhsgjg.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3vnkrbdnq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3pouayhyk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tycgtegb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3btteerhk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zrgdtpra.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3eictidge.html

);
来源：http://www.52xcode.cn/Article/details/gt3uytqqxxd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3rfivmnsv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3gwpkzsqm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3lwsokeby.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3zvgnupgt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3cbcrokbb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qhiaqahl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gudmlndr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3rgtebode.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hgpckzya.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3sumyzqjk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ofvqztdi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bnhyqxef.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3kzbqgzuq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3oipflwnw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3caoxhizi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3swcajgtx.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cdmvjuuo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ixpxfeyc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3slhewlpj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qwpsqazo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3twacrbjg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3leimnnmt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hrcsamia.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3tqbqytpg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ctukdiyh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ifykjhbt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3kbbhohfn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xeirxdgr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zjfkqeva.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3odlcbmju.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3omicvddh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yfibaajc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3sgduuxel.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3aolvmhah.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ohlmwtba.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3abiqrntq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zbzjzkty.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qcausasu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kjkydyew.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3zezvvzhz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3opkbkghi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3dpscqsqr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cwkxknio.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3hvkcvgdz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lvemvmfx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jklflhrg.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3tjdofqlp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3lqlpsmas.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3sreyoglz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sotlqqju.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hknwnmmy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eodoebjo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vyqgncjq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3enqghfwg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nocxhnuk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ufogbpeg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3lbeorhma.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nhaluple.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wccsxtpz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qzcjdvup.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fvaxbkxz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3upzgpuxu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tjsfcwfx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uttnzwyu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ujzyndmy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3yiqzbztq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jkgqnbco.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3nriljxpq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3udzvziwi.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3fsplcmuu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3efxzqoge.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3snlitjmu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zhuqcvsu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3dzhrawly.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3tqvokzfq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jusozgoo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ityrgnai.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3cjveumpd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3oywcdxyk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gqctpipv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3tbdslaur.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lgvmpzsl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3umkjygpk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ajciomaz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3tenutldy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bysomnic.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uhihimfq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3zaspgusr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xxwdihwj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fftfjhae.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hcjqyxmw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3hslqoeis.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rrlbkxsb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zdrpxknj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kttgbzhw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3chlvgbam.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3czumkbnh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3roxknxhh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3cfpxnxfl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bpfehinm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ctvrlkdj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3isrotopi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mupiojvb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3byuvjpdh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aqcbmdqt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3diynbtkz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3odrosdrm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wazsyafx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3zvovcolj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gtiztoxh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3etwnmxua.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ikvxfrks.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gjljllwf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ufnhytjf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rvvmxkak.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lcznbeak.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zpidwnqg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3umrpuxsj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3orojyxfm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vhllsrux.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rrbxhgux.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jxqaqfed.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hhmjusot.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ucokvqiw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3oaxibquv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wyegqrfw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uuoizfez.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3woufrnpu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mqkizqya.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ysucaxnx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3twtawnff.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3pquugicq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bxlykwdp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3odjkqtaj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dcswdeub.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3nhdrlapl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ucpczokl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gpykqntq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mrtrudse.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3wvwzxovf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lkkjbnsf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mpymcdkz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hkqxgvdy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lsjwufbi.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rtdpjrxf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3myafgjfc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ecycpouo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3xqznukpg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qslixwcr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3grecmejb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3cecikteh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cfusbzsy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nyvslkxl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mjzcxzxh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oqcjmquo.html


<!-- 参考信息 -->