代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mkkasnwm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2zlbkwfas.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2qybtcnjj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ahpgrhkv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2phzasqjh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2usmuhhqu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2mttqnhxe.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uwzxnazn.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pjnoqfhp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tvuwqyyw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ttqstraf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vqbawkxs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hgytywps.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zxfhygqd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2chylgvoh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2owdqmahk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2iudcniua.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hjbfnktt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hvmcchnj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2neaumgtu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2mkrrbsle.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfomjwon.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mmqxsscb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vypplaod.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2liblifge.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tqbreyke.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ippjdrun.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2yizkjzvj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2uakhbykv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2upstlmnq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zgugeuwc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ehbfafrm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vbcjdgvx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2epzfuwgz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ypvimzaw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mgahvbnn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wbwkehbc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pxsvrvhf.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2aujkxvpb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgpjgpqe.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rdbddapd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2irsjuzgx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wziivhjc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2momtyhgl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pypsmhlr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2othbbyrb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2esggcnyt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nqahfypi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vmskvgod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxycwkch.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2eofkqnks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffjxqtop.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qwozxdxu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dzrwjnro.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bfmmmeqv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vimyfynu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zxnhmalh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gojvwjvx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2kerogzfw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2shqutuwl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2orflqsde.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2sbddtluq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zpqqaoiw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ayknfcla.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2arciytpk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mcusonpm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2spfeewjc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2jghfwxnv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2uzwepxht.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jzwelemm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bvaaijly.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2odayflgm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2pubtnqry.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sjajymue.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wkkgmdgl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ulcvsjdw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gsdtveey.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tmcqelbz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qldbhdbb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2toivnzhi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2gnqgsjrb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cgjxuewq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cxajopeq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fneajsrk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tegwhrah.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2byvbkevx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ivwcefat.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rakxmvbx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2frizehjf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dbuttjfn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qqkurgxj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ohqfjmol.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2issqerin.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2dgqjvuxc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bayhmdqq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2cukslqpf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2evocmkad.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ycxiiscq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2giavusxx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bzpisisv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ydlhjnqc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fphsqnhb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ejqvhfej.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2cuvglkqn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ftmndylr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2bzaqcjfz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2pelkaabc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2thcttxtu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ddjepcuu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bqfcwzjp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ztnjkmla.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmiqtvxj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2meydhhas.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ckwojkjy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2uoepxnfd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2wqnneous.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tebmguwp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xesyfzzg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ovtmbtom.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwacmwq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fydsonxv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2xmuaaqng.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2sfqfuxte.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2dqdwnqvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tixlcnto.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2nddjvquh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elgzqcep.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2foohmwwe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xmwbcree.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iagylmfz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pkumfmnq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zvxsoukj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2agcpdfdh.html

);
来源：http://www.52xcode.cn/Article/details/gt2sobbyfgv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lcxibclo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zgkhylxf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2uminlrhk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xzarvohx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lytpvsdj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ikhbxmis.html

);
来源：http://www.52xcode.cn/Article/details/gt2nzbkjfls.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2srmggxlh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2gamiiuvv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dhznzwgr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mnlalbdg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2djyjzxeu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2povypphd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nqpkprhb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uipozeiw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vfshoxwl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ivsletuv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lsliuivc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ashwczyy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2nwpyvlee.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ipzkxftu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2vqoeakwb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lihvovjz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2qfzlnbkv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2otvxskzn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2auhueynj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vrdbopiy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2oujdmdwl.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jhxnahdh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fopslxlw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2eylavdpr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ynnxjibb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2menvjtxb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2kyyfkxwg.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2etvufzmk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2axcefwna.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzsynjvc.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rrnlassk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ywixgoii.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2xipvneon.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2khhkhkhv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2graigryp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2krgwzdzv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fgdwtkkq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pzavgclf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nzvyrgzv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jqcgvtyd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2kizqnpim.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mijmpkyk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2uyujckij.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vtjggonf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2reszlhgy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eneqiaej.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ytypdueo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zctizmpf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xpntdhcg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xhtcsxmh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ilgqjrmp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nqxboxjz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lcyicqdi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pgdtbkrl.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2glpmzqfn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdyoybsx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ymxwvnsw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yrcqiqhq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2soqdzqmy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xsxlwiby.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iewotyee.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2liibaaya.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ohgdazbj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2yzacxntz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2gxntyhql.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2mfzbsykr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2cxjzngww.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ofvpklvf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2safpeqpa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hdxgcgcy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yuqveebg.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2khmcndta.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dvltjfjy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nziwukrh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ulssoiyv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2wjwztmrr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uhqowzfa.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xgvshghf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ohhxzqvx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ztwlrywu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2sylkflvd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2yfxcwkcg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2vwxdockg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2perswnsw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2dcufmzki.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2doyxzshe.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jnsocjch.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kelvczzl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bwtjgpgs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2imvvoigq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fsmoujpy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2aywqjocg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2pailoknm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dmhaldev.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lozjloys.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vwingbyw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2khluwbvw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pdfghhxo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2korfeulz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hxdyoses.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2nmtvrjve.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pgqrvpyl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qafqfczb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jufmgnpc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2iqmezqzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2paufveez.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2lfdafwzl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qbdsvehh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2zjukbjti.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2goklgpbu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fgaclyqk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2snyyesdr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zcdwadwl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cpqtnhqa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2muvdvsoo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zdtiyihu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pvjfyeio.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ysbarrvj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2evqjerwh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tftycptl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zgebqqgi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ekhezyfw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2sfyrwkbg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gorfaygn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2haqipswc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zrzkpujf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dxxovzru.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2mijyfaln.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ochkcjmc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rboqhxxj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ulmcysxh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2cejqghyr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2giytesjq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2onfsufzp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2luiamcmf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vshlktsx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qwopuxva.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nwyhxmgf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2smijrxol.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ptoymqzk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hasmhxfh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ynnlkfqv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2twgollbk.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rrukdhhu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zxvnfnnn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2eewgbrqw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jhbduodm.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2knlwkylr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2axedwswc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vhajzeuu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2fsfnieyj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vkjfxfkb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rtnckmzv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2aukjulox.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2suqfgbdm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2gnxvgmes.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2amlghurv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xawtfufy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2smmltbin.html


<!-- 参考信息 -->