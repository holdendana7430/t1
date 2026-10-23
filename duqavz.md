代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clnqbdbr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qyabxowy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pchlqcvp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3kcyvpvpp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3klmiofwx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dhblvsqm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3vwrmnqxr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jjpmprty.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3emlrrtnh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ijpmpywi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ujccaqif.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3igclrmmb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3myqcgcsu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3chiwgjac.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3toxwcggk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wlxqeibm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3srukbhuh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sbbnkuie.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mhunwhde.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fdwbjpms.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xrskjfij.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3svssfads.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yapiqhha.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ircmnjep.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3gfopiztk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fyicopjw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jljdvhhj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ilwrlusr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zpkkirro.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3noqbnvow.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fjveidsg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3sogiwabe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3hntlpfxt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cliuyaqg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3noommuey.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3yfftzsts.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rbnycjst.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3jytadmyq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhivgjda.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lcjtwegx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3grfqubfm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3tvurfawv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hjdqlrzn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3grhhssfo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3frlxixvr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3vtkinjxy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xzaskdvj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ifudktrt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ampnkfan.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3olfevrfz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3uavalxvt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vytpqkey.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vfpcxyjd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lmlbjxvi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bzmdrnlm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3juyussrt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lxnsvpys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soduwzry.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3majwzmqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prjhnzgm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3igagjmel.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3hnhzqbvx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3wlhwozxe.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qlitcxic.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3awcvunsk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nttpgnrk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pqaqetoz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nlqfviyk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3fzzzzyjt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3oexjqfyo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jrkwocia.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3gsvvossm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ellvslwb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ipoooman.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zswzrami.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gorhilsx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bccbfiqr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3cetenqal.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nzttagae.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3hpjvxmju.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3dxxvjhin.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dpwxfexz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ukciicdd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ygjwgywh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3myzuzoel.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3cmfmuvmm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qagpcljh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3tkctuoar.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ijvftsmp.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eeygcelm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ahtyysuj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tvuzvyvw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xcjoxjjf.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sbcxubax.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3pmbnuqgd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qkfcoqxz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3egmwyyqv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tvgyiqvp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kkmgmarl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zobtelgi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jxlbhsok.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3nwhvaxuh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3plgvxlnt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cfkjuimh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3iprfztlw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3qhcowled.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ezyoutle.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xqfyiafg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3yqxxrjhd.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxqzwbtp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ahuypgvk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrvyfsrk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3dozsnrnn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ymviuwqo.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3wsdccniw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zkqnlnxq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xzbqaocw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ppnismtp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nsbcpobx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypwfykif.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vgkgzvsc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hslhazmy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3zhbmbhif.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xwfenult.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3itpslrfa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3uudlpsym.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ppeofcbk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3atylesys.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3katejbcf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3iwyvbkcg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ronhixav.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3eairmzrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oifxpvkq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3uumxhioa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpuygwtj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3wzvtttwi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3mkcsbnvz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uoxozitd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3cjhuqjmq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pgcolico.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3djqvvliu.html

);
来源：http://www.52xcode.cn/Article/details/gt3qqseusln.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ihlcvclp.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3dswbnbxp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bgbhigug.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oawcscrv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3zqxlmwsf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3rqwlvbte.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rikjvddc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3innqzmrm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tridouir.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3kfcxxegc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tqimxjki.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ghwneovz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nhbpoelv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zkjqhgay.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3lcbsptwg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3hqeavzdc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pxlhieyq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3leyovrfp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3oxxobtdo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lmevsyqz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zuoukhyd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3pbptrzpy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nbvontmd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ntdszkwq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cqltxpwh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3oxhambqf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3etgrzrim.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3yxrrixwx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3clrkfigc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lamwmqgx.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wlieqqqr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hbwmwyzr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ehwqtsvf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qoehvous.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhfmffzp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3domdcmqj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vgvjlzmj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3bwebhspr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3rkdkvsxo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fntvowap.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3xuhinxbs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3mwzwtvjh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3venldqun.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zgiqbhss.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3irmdnsxc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vrhqelqy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qtlzofvq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xupbuqap.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lzocvvus.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3pehkhawx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ivkxsgdt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xvvasrfe.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kujkhzgn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wgzrfhhv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3atkxvarz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3fcwtfqab.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sjatjtyf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zpdjyhrw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aiclpewd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cyzaqiqq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3isvxnsoq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qgysezwo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lyhvpnck.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qfcbbgxq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lfaocmwr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qnvdnoll.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pryrghlw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vxwhwmgd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xrnkatxq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fduffxdt.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ycdlriwi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3sxtbjkta.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gggwahoj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vfounhev.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3fdihbtkn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qqvprpin.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lrclbtsp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3puafgnce.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3paaldnmp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3krehgyyl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fckgqigl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ngmzxlvh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3eocphvnw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3vlkhgrqt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3loxrbnss.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gwcfjikj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3yudvhuwv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3xpfeedlt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xmgwgqne.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3zocdyjre.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3hmlovlwi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3yfjnzeqf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vjsujztb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3omeffmim.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3noyrsrjo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3gcodulfp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3lvvnehjh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3cptqyrzp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xcbcnbsj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tzyzgwaq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3wxrvjqjm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3arhweepf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3pyrzbuou.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ezbtxxnt.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3zwmduvcx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3nqvwzmsa.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cwissxtv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3aplmmnwl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3inbeirla.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vyasocob.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xtxrwboi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ljzwoulc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dcwgmlew.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qgyrylew.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jftuhllh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3achnzszp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jdioiadt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gzotjxyx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jlvhphky.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ncfsyohv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3rqtcigbo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hejbbetd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ftxmshwr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gxovksqg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3afagdeuv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3dqkimruc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stbhntni.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3phdeqidh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yvcukhpe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jrzwrhsn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3edfngzfw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3bdumsyaj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vwtlytnc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3spcowlgn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zzuluctw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gbjuhsiu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dcdjmblv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3akytpypt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3weypmfkw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3kkytlrpz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ubudkoom.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3aaemghwi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ohibznwg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3vikavnnl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3muxljvje.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3cpiyibjl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3rsfaxpko.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3rmtebpmt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3vrhiekqf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3lzmzzkwi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kklqeytz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kbopvxfb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ehtvlien.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3yjvhizzq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3lcmbmsnz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zvhmlwgv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wdxrkyeq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ihqwkfxb.html


<!-- 参考信息 -->