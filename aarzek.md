代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3crapnyjg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrxerkpw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ifebiwzy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uewweasy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lrycuyay.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3pvpjwtay.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3gfeescct.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jhsukduy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3yierktoc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uhnccqqc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3mcpqvwym.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vdenywfb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jpkgoxyx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ulsfsztq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3pdondeiz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hasocmvl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3snapcqrm.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zufbvcgm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mhryhudm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3odmyidvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3euielpvx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ykldzszc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmggpogu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rflunujk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ofszcaim.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mejipznw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3khwoymnu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3oijjvldq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jfvebxkz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwyomzqy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zhmhldgo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dojigvyw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bavlhoan.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bxhtrdeh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmjoutni.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wijbjlqu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3momfvgwm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zsstzxrj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3phpgbtlh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mxmusjky.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ckolapkt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jzvujpez.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wzqcwfcd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hijkkloh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ncynwpiz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zjelkffr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3gskkxomi.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qabhcujk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hamhxzei.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3nytrdklq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xbfxidlb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vytimwrc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3umdpqbwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmxewhre.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3mzkgqoun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwnsvapj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ffagbpct.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rzbvzikh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mxxjafht.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dbjfjwnp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zulxkztp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kjwtmixt.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3eqsolxqr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jprllrph.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hdaifuuw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mgsarepx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qlofnbni.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cawehdvl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zxwibpwe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3vhliqtos.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tefatjzo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lpjimgjk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3lfijkfdf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qkamfmcc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bwrujyux.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wddcablr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3acuxkuyf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fqvnxtye.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3crgtfihi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3twbwyxlt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bjwuudau.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3safsaeqo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3taxozcba.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3elfofaux.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tciiflhv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nktglmpv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3duwvrgcu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ddrowybj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3avuermia.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3taximkaz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3katcvsdt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3suhuakcm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cmkvdxcc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3lvustsdv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bhyfpndd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3moymlknp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3schfkzgb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3dntjbhvi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3twqlddjb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jnuieecs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vkjpsadf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ixzytekx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xmcbhgis.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmfehekn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mdecbdpx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3bunfvhyo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzlyhxcm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3uypfytla.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3agfdhqgx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3qjhwxjza.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3fgogqdbz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vubfpkxm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3oxykwjjg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nirhwamz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uksijftc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rwiswgmp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3acapwqyr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ofimoizh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tzgovwhe.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pbrnpdbw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3clumngck.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3blsluqgo.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3kvnbyktf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3htuooetl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3veardzlz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3zhbrqyjh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3sunmcbcc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ztzqpxoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtjpyzxz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ycnglmva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dccaemjy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3kvaoxgoz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3kosfknch.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3patxnfcx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3uvfgyzkj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wxhgggmo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3suubmpes.html

);
来源：http://www.52xcode.cn/Article/details/gt3chiejdht.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fkawcyqd.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rwkamhph.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ickqzlzx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lpxybqqd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wfddsiqi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3cxylqder.html

);
来源：http://www.52xcode.cn/Article/details/gt3xqmypvxd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3pltqohpz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3jdtrlism.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3eeuyysxq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3albaqdsj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qhhnexfh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3eyzhuewb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3ehskckuq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fubuyihw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ocdsomwa.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gjxvgqfy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3uhuzhjcv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3dgiyscrs.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3wpnawnuh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ilegaemy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mpyknqzv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ljverrqw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3xptqbteb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lxsgxgiu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3baaugdxu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3veoaivyu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3awtypkya.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3sdrjrhxk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qanthgnh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dpnrfybg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3vdrwllom.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gvxqvjgx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3pllpeivj.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aunolejw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tckupxty.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jbxoyrcx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3gbyoclho.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ctzuuarr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3nuswtdem.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3sceidnea.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ocepkaji.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3prgiwxzw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lrzrvxxq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3nvsejjpx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3azoochjc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3krnrcyht.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tbpjljew.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3cpdyvofx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3nbeciwnb.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zwayvmoj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qikqrrag.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfpidhiz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3vzhszogu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bwpehjse.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qitfwowy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vxozduib.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3okjolcwc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3afamlvtw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ojpxvdxf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oyvmdywh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3phmgaqib.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjdxqoet.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kqpieujy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3chealdxy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yzwrdchd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ljjhkpyt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xszthems.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3refllcvx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3yfurnhyc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3pwnnkewh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iotiioca.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3eaycblkg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3colsvpsh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xmvitgth.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ywdvcvbs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hikhhzji.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ejhgcsdh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hfemofkk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yohugiil.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3icjmehvu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yrmjfmgx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gfgajisz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lckjwofe.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dktenapb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ltydykay.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qbbwfxua.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jejorwuc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3mwclqbui.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sgwykrxt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3gizyiueo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vasrxkqr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nmgiqobp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3mezczzml.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ctcsdwzy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hjnsbqxl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wvkavkuo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ricgqadn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qcxumfzg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3gavuxwvt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kaidprny.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3friijizs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3clasvhgl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3awaavkoy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ayesiaid.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wafuagmi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ehvhpbwc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkdurze.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3roibqrkn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3auwlzxrf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iyvqewue.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3yfbmffep.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3euufulzh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3torthpwv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3lutjlflb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jawbgvbd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ujtxxtqw.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3edrcrrdd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3epzckljg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3rldcercc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3bhvwizag.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ywxesoxm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wissramw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3eefvvmky.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vvsoefdx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3plhgxicf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iuuhqivx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hmkjneod.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dfbrcpix.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qhwswytl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jwhbrnin.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3layzolja.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3yiiudpcz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3linuvpub.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xvyqkzqh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fgguwrla.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3htnlfpmr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xavgurlz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3fwfbzcjh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jhkeajiy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kaldpltw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3iadkmwpu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3htwvzqzu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ulneaedb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3smnwecfd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xucjofiq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zfuofesl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3tlcspjta.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3simuroxa.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3vkjihzpm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wodkndto.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sibevwmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ibiovfkj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3qxvjldqb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nlrztvaa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3pzpilrpg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3woubezke.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vybghrti.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3szwudcki.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3umkryxdd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sujlyxdn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xydapwmd.html


<!-- 参考信息 -->