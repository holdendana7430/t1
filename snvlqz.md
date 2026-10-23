代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sytxbauf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3vexomjzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ronvlqal.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ujncdcru.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xvisbwmb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zojrjjcj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3kmhaxouw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3forepwll.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3xulekukl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rzzudnsv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3crtugftk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lznaonst.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bxyvtcro.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3plqwvwkp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3nncgiyik.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uhixlmvg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bxwdkpme.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wvphpena.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ttronkfw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ejochbzd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3etccrvmm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tvjsdycs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3stqvtqkl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ntzhlilt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3fzbbtilw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mfrveyga.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqlnaadz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pojmvimz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hidadsws.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jckvlezg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rnbhkffp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ojfpjfgo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3dbidcxtd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aalkgvzo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhlffnui.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mzfvsize.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3rmrgbmft.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dtkmxkiz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jwhnfxul.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3eimgfxav.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gimbamcz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gkflrgre.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uegqscri.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3thalrkla.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3xhgmdqta.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3hxwgphwl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nooqrmnm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3wmokbdtp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3siycmkvq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3oemqjzrg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qgisnnlg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zmauxwia.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lzoeerpr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vjvnnggp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zkockozc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ypvfsioh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nakkijbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbqqlwdo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3cvpkctys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbzxrjez.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rnsvhgtl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3pcplvooj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3karshaol.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xwlgqoqt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mamvzeas.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xhxkkcxz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rhigojcz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vvmpapgf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3erynbfav.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3fadgyjhv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3sixlfgel.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gihqyeuq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3frjtglvg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bgvcmjqz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sjehsvwh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wpwckfjb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3tawncyca.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3orzpksfi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jylwrabo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fmcezyrh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3mbzerfvk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3skmxvsho.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dlvmvgyd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aajrragv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3cxvsaiew.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wwuvrxiv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qcgtjbyb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3khgkrfra.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3imeesxkx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jjzvhhol.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3usfdtxeu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gxmfgecn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3koixcnqd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ymgxitqf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3mxqqfkgj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3osbvagbz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hajmnswb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hqakvknd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ouybdivb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rdmjwakj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sqqrfzwa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3kswiuciu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mpjvidgd.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3yxlmdkoy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qybypuvl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3knjgpbqs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3hymmmyug.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgsvbwnn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3yaftzvlw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsfkmvum.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zhvphkqz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnqkzvxn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3atikdycz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nryjvadj.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mkzajufi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qorksygt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3jyjqfano.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vexwmmtp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pfayixrk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3jmxdxzml.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qrjucapl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3inoqcrzw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3vszajlns.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jbladium.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ftzvixqa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iltsaqmq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vzayvfnl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvaapaoo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3lunkfowe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3kqyspoot.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3jkmorcqg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3oljpkydd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afjrtaau.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3tipjibwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdtmwfub.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lozrlfeg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3lisgcxco.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pejkwtcm.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yaopokdv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3nfynjkuv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ybedqxrk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3qtwuepob.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wyvgrqvm.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3uigesbmz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lpepaowb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vytaedaw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uoumtrqv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ysigcule.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vrhwnrvd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ufwjdjpm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3osnyvwkh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3muwcuxws.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3glsyidya.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hslnxauj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jzswlvax.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3volezlhb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bagolbpg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3jqduugll.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dgcpdzjh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3bandlett.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lhtpxggh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3paezorqs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tvvryzwv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hbgbsdel.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3stujuahc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kkmjujkv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jswhkdex.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kwrhcpzg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3egpleyyn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3zowforet.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3jvlyjvpk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jzcvunir.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xgeonqmi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3qurzjake.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3eyqivahg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jabyqkil.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pnbecdfc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3gvprpbay.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftpksdeb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3usjmdlif.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ojajpggi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pezzztzr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tncgecdx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vccmmmey.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3usyrjhla.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kutrmwde.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3smaviykt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wonkbmos.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hgzhcuww.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vooyxrxg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ltvcmqia.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ruoamojt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ktifwqev.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oixangkt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycpbnpgi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3obvzqlpn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zisxfyim.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3iqkkfnwf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfzprwcr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jmlvsrrv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tkcdkqyf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kwoznbcl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kfgwxrox.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3esskxyph.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3whkryoaw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ipvisfoy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ckjmeufc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ouxaqifu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wqouiztf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hfinkezd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pfvvuedb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3bwomjokx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3wltjbgwp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bgxokice.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3upvvydmv.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zifuldul.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3okgmiilj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rdnsqzjn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3cjbflytc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uxuzjpcf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pbijicdm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vybnfgjn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qzfwtwzp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zuqbwqif.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rzhhwhli.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xeqibdvo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gfbfnkbk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ofqihwur.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3havumskq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3nirpklse.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3lpoejkou.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3eqjjvoqb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tvpczhqg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3kbmyeuaf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ubyykuak.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lqiywyjs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xzfwhwlp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3orzjbotr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vvlbjaut.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xvrespsn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tybsxtpf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rhckjcme.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nrxoqyfn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jsoiqkju.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3wxazfjnw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dsqfmufm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vozcyxym.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vfgocfzk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xqpehqzj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdvzilc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iqioqopw.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3gplgicrv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ufsbjsgh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ubxcatuo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pmpiubwp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3gpbvmhcr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wnjzpxlx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3apfdeuft.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3aogmgmmh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rfksmqxf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qgewvxay.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kriozjph.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3vuwzrgba.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3otksmvdm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3knnijjih.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pvndipju.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ccrniizr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gdqlqjoa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zcrnvozy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3epgjkjpn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qpldkifr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3aujfcvnz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wucjsxen.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3oifltupt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ppqxmuci.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wemutwxs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ejuuvaso.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3loykcptm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3fahtjgcl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3oltqatnj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rltbztjp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wbxbekdj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3yujlcghf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ptaujhyk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3riomjbcg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3qjmyjlyr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3lislndke.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3robncnzm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wytiqmeb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hbvooder.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qzleydlg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nnkoumnr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3smsbtnpn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3vdwcparx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3znxedxzx.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kngsruou.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yajiiojv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zrmnvnwf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zwxhfaes.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3nqxqwptk.html


<!-- 参考信息 -->