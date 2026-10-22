代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jddhwilz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2zsxonpbg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ewwfyrui.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2iavhgizm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpierrkv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2snsixydo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdaxbvsf.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ealwhzli.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jwhfikjh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hnvirdig.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jamfdykh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2havdpgwt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ggluplvr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nmzlgbok.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2srgumrih.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2odnmmahp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2yslawgbh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qazkpsev.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dckxrjlv.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iqozaoim.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gheqgzka.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zutojbvy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ihcrunkt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wjnpykat.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wyrravpk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mqxptupx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2mmcogwdw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2iiqysjgi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pclpzyfb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wylxguyn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhnpsezd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2socofzef.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2csskhwak.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2edcpjqvu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2epceroub.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xbpqqasn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xulnnjpg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrdoiuko.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvjihzee.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ydmhzoqu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2mdznyzzl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hfkbwajf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2uwrkvnde.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2buodnkmk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lonacwwl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2jrgmrtkp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gpcdhhxx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cyaoddxr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2tykslvzv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2bqpmherf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zarruheg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nskykmbh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2abomhiqc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dohpxqic.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2nnztyvzp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ohpwghgv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bjyaxavu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2foawdsnc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2juqsvuvc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xzddjwqj.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ohmcnfqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddxciwuf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqtvrxjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqugpsjb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2tjqbawyw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pxivkukf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2okijcbez.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uezkuegq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2plnalqja.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zthsaagq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qngenthj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wxwtywsp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gedvbrly.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2qeskiezr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dcdbtryl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qqecjfpa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ikohsdax.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2izlyttsq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2puwwzphe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ynyoshjc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnpputpp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ffuqcemd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hctlidjl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xlhwhpkn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2fyxzddgx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ylpqeirm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2aqkoqjwv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rnmxmpww.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gfiluhff.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2lxstdkte.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2uxioyzyw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2eayitvkd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2pogmodlj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ehefyump.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xkqkmanj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fgdglaaq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vfwkgjut.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2kuwmjmhm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qykmidjg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nnzwvdkl.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ljcemkmq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qxfztrqr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2sgcehrbr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vnwjhewf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vhnvpgvl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ewlikebj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jvfrteqv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2aatffwmw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bkjiftkc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2flqldbvc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pvgztsnx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhckfbuh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2schwmyct.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2mnwqjuxp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qrwpkkkd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ifxaoubr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2tdhmkiws.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nzjrvvdw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2qfruqslv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vfjwnuuf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2utdkqjzp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nrurrkja.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nuvoutdy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2uzfoyusn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2kzmubwnd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hdqhimgl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2yhudvliz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jleojbni.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2iuaqswou.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ukdfikxt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tchoyflq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwsfgfnu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ycpergvd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2zburslnl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2retwlogf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2djizzffc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlrbksyx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xtuqpnvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xendqlwj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ewyfydnb.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2qqemoqlf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hdalwswx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pnrluevl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zvtkmwbe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zutemqxt.html

);
来源：http://www.52xcode.cn/Article/details/gt2jrmfkibz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2crngrmph.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2akzmdtvp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iayfjvpg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2reeaxfvk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ottftdlv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2pxcvoavb.html

);
来源：http://www.52xcode.cn/Article/details/gt2gbubgjdb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2gxdnkiio.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ymhyecqh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2qhkyksri.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2naomavjz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2aiqbevwj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dxhhhnie.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fzlkvves.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2oqzpjaqc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2wxwcteho.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2nuezbjwh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mzydmegj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hznpinvw.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2kjzikfmx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wbpmqcaj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2fbbfmxer.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dbyugqum.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fhmqsixg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2eyuiobia.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2yhtbikul.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2yrcovpyu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ynasqcrt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2lwswyheg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xqdsppmv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mpjlndpo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2acuuqxof.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2xjkksloa.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bhjuduyz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bgkwkowp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2yuwiyqzc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdnabnwv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2tnbnawty.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2yeqoidqv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vllkrbgo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jzteeelm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2fuptyldz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qbvrevcs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2onoqwozm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dhciqqey.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2sxlninpe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ffcwilri.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2pohtoory.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2drtmjvsg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2cgvimdgf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2gyxzjkht.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gymowojv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vrbvukjt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nzbulwse.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qfdashpb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tbejmpso.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2odtaxtjp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2yvztcnnm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cnidyckg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2tdpytlrh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2laiodzcl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hypdukpa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2biwxmabb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2zchasaen.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qphvctvd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qirbyvyx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mypptxtg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dzfjbwpc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zrbrgeiy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pwopjhzf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2izuyewil.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wglfqpzx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2fqhxpajl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2pmhjgxhp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gmbelqva.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wbfnwkpi.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hxiaknbj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2iyrtdmdq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2toxlgkze.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fcqzegei.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ifbkvznw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kygtsjxo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bckzcovp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2txfdvdvb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qjmkigvb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uqbjiygx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2stxigjmb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2yqaieffs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2isnaxsbp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2jnbjriyb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2mtbwjtco.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2lbmkuivf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nbmuscfb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2eclbghvk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qqdsywer.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hrbhffnc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vkmamuag.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fvqjvicl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2oaresjll.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rpomehtl.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2oktsmzag.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hyywbaui.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2nhxovaxp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wjkpazko.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qtzlubyu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mwfmraat.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2qfcjsufg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ijizyuyl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wizdbflu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qvyurcjp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2urtjuuqb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2njlaaavl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hktbhpmd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hudvltii.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2dsnrtaac.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zypcwwev.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gbdgflsq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mjcqvvbd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bbbinkcf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2xswptifj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2kuwvhafj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kflvqzmg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2njtkwucd.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2cqdsvvkr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zoyoaqqw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2duhdesld.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2osabutoe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jedooyci.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xxvytabe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ssuognqx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qdizlame.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hflnpppb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ydurzmeg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2phetqgtx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2eyrtcrpi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kyzpooic.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qqggbdmu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qwsetyxr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2evxbqtpa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2thneqekh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pzotjsvr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ncyzlzru.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fbsmkjin.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xxvfulal.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2kfyknjvd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lrftgwrq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hphcmslt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2oyudblvb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ocolqhoc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ohymxvmi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2bwqspqad.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2oxefwjcu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2kocuoyaj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2rukhwpya.html


<!-- 参考信息 -->