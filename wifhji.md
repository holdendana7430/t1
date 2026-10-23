代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3keeagcyq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ggivjwiu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dckqwzvt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dptcoxej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzinzqnm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bzngyqun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfvojmks.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3giilbgfj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zasdxcag.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nifenzsb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dvwjqvsm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3btrzvigl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jhtbjueh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3sniangnf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jwnlecin.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ocvevlgm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cwguwnlq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wzbxsoky.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3guosxtdv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ivoriums.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3imkqqknr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kfgvlawl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3yjfogfhv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3vsizuyxl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3umfjkfyn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3pqypjnwo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rizapzue.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xxaczsja.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zznpospf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3prhaqgyz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3izntcscv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3snikpnjk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3tznmmltx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3eonayywt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qxeqwerg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zootviji.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3pwjystcd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nmxvhmga.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dmkqknlk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ruyekvit.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3aymknpvx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3txmgilow.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fwnozqqv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hbjtbxtn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3eucdesez.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3scnlhbra.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zxxqtunr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tzpobfcn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3lrxlrybt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wjibrvnn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nssowhkk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3pavjbddk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3leagtlvy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3nipfybkz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3khjjstqu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ersywqoz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3etjytvfw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ebjrrtyo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ugwdsdua.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3pthvggqw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3shbsyczz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsadwhyg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3rrzzxtya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhruflnk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hufjcegw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vibrshao.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3pyxpgquu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tzvxkmvj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uurphweu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gmlafvpu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ndgmlmnh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3zrxxotue.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3obbzuwxi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3uocmlfay.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3lpzmltwl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hgpicovd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3hfxdlrgz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rikdejtc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bwziyaao.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3grxrtenx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxdxyccp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3eevguedx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qttlneeu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ngqmoqjh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3pdlpvrpt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wbzjvzry.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dasesuyj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3flovvrrw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3xyilgfyh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qqcphsgr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wtaxogux.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3aqkkaezd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rlgfabbd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wicvvoqz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sqhnviop.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tsckgoef.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bgsgbrgy.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3bcrjggsv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kugouneq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zfkpdtja.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3pdyxdeex.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3rtnepsqt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3kevlnffl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xuniundu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qlssgxxx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3gmyfzpki.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cetqykom.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ylcbdytw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vsloekxy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gxyotrcu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vcmskpeo.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uzatsulr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3higooilf.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvmllzsv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akmzjscb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3tzexoluf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bqnzcmlu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dkjyrxzs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3smkdgyzd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3txbinhls.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3iozehgol.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3awdfofxl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vyujywbt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3gtguxtfk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dznqmdpu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dniqxacc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3siifqgnc.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3nltbiewh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3lndbzmxx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uvaykbli.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ikeblcrv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgzpnptb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ngvpxxqn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qjycgprj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sejphfox.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3rmodicuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wscbsumh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3coxqrszb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpuwwthy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vjjydgop.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hogsqmnn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3aqfvxruv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jwtuxxam.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3uoqoqkfn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3yelbtmee.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jbrchcwo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ccqcetgf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3nuaevlhy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hkxpbrhy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3snxeajkf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cctzrjbn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3znokblqj.html

);
来源：http://www.52xcode.cn/Article/details/gt3yiumsbrz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3shcqkkfb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3dbikjtha.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3tzrnvqug.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bokfrlqe.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3blrrummy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xypeyrnl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3yanublwg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ghhxefju.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tewpjmpl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mzqynqng.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3uudjirqd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3iyhnkube.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3nwjbaour.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gzcskkrk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3fafkteok.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mdykdqcw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3nwqlxtya.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fntttsst.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3fcgzgygv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3esfystkf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3huypyoxa.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xscuieud.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3cpwbjynu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3mcrnxhwp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3sugtxvtm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3sdeodnkk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dnuiphzl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgsxzibn.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hphwzdqr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lgznvmrn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3loyphvsn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ocfhtzxn.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jhsuaaaq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3yqwscbmf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3brkznbxb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3uizfxfml.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3artgowzk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eabwbywq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bprigzec.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gkosfilc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ipowwjue.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ndgoaqxf.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3rextpgkk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mbgkeaxw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nvjvjtoj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qlqzswiw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3urawqino.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nhucjweh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bfxjcygo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pjnchdzu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3adizapji.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qrynznxs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3drphyahl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ruyzdyir.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mxqvmyci.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uqdlmzsy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ylsibxwh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3eommdrnf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3uyzopwpq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qcxzspkt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zvgggbnh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ivziaggt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qzxjlexj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3hhgmrqls.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ppfugzty.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3sgjjpjcx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3rsveygvy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ggiuismi.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3gxhsjzjj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ayhuonza.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jlawinvr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zfapeyoo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wsfhkqfl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tljomqxr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3xvdcdxbj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ovauponp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sooptwmk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3cyjgnmqh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ujvnjvls.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qcbiwlzv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3zspplfpb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tanvbcfd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3tflotwdu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3uhbflsip.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vkwuskev.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kiwszxzo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mhmhgytj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3rfytrnpv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wrsoqujs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3oblpkabr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mmxaojob.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bgmurlpv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3sbfjfjrf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3eqklelex.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hisjzbqi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mgbrmmdp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uesjojbe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3lwwaqcxq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3igwirtbx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lrnkrhwi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3edhpyfbt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iihqgbea.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rxsmaivn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pugylwjy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qycndyom.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3notejuok.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dreopbii.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3bhceueka.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xcnmzdlq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kntogsfm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3sogdfbym.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mrtspdef.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ptxzqmyi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dokeoxxn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lhyrdvxw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3oekahzxs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kzqbtfjy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jlwmonaw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3upogdymg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3msttbcqy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xxqlyitu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vepezbjd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tfbgtipc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iigcqjzv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fpyvawjd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3apebrqfz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3opmryamm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3oersrtuc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cvtvtnac.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3qzvjcmse.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vkgjmtsu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3owdorqps.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3fyvuhtvg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3nipcbxxu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3svcwaykd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3oeoqckfo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xffyhzaj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3eojctjbm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ztmxkpwa.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ozrkkgnb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hjxoehwi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3njefzliw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zufbekah.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3axdhbcvt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3iqemdtdj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kpwwawiq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3tjawvsak.html


<!-- 参考信息 -->