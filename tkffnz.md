代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hchhkhaj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wtidahgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofznfete.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xftnofec.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2khyvzdfm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2fhyvyzvu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2aeowjadw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rfpeygdj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ybuddirg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fevadhji.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dzhhopma.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2soglznrp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gqafxkma.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mxwinmjj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2uprkbmly.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ajdwppnr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bajxfsdw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwxipni.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nrxpukem.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2cyrfpera.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zbjzaaes.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nkqplaax.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ccxovnlb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2moftwcco.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qkodrblg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nedbrbto.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kqhvicot.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2kxswdasg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2cnrmjzjn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzeoffct.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qevbjrbm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jplllsru.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wtjlangb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2npitnpkr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jbvsnudm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2efxdowes.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2wpjabhvw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wnxlxyvj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zhsntpux.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hvpsrtzk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2lykuijne.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ufstqmfj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vgkpsybw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ebmenizt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fzrwfcku.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wiajbpnf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mpuifrpi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cjljzkor.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ygpshgfp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fgmbcwxe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2reizhrdu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gsxsjqxz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2simmvvms.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kxbsnjkl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2pixvrbwf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2vrvdjwvf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2eaiwmpgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbqqwgrx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2metqcfwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckrslwym.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2btrtjyoz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vtpwbpee.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2bqzrhgsp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qjbnugch.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xepyvzka.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2nvuaavxg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rbxghdbm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2exhljfgl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vfkfauqb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2cwbdwiwm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2eoyyuzmk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2qhjlphos.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hquiugsf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2spsrbbvt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yrqqxpfd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2nesdrziq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mhuhvdoi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2udoinqsy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2yitkyxly.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2octswfrg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2jdyfwjsh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pyoodtpe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nmcbouyn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ztrisizm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bniwpllv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fnznpbla.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2gsxrokof.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ehwodany.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gyiepfmn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ignbsuao.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2oplmbzzy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nybfrnho.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eionqqdh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2tzxzeqow.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2xenzndla.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vtjpdabv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2mnymezgp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2hipiopgd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2fyedrtls.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tyuxehqs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nstmcdpl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2uleoyhnx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mtnmcyew.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ieevsuik.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2anmnbdwh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dpsvneit.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nvcvkhwj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odfuahop.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2kjkvjixj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idpvwxql.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dctozlyw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2rhcbhbzz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2vnhkdhhf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofuueggv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nvcgmpqe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2kmnnufqf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2xytruwtn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fxefxgkl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lzapyors.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2khrbjvyl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bhbuyeaz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2noijihqf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2fvhbqyeb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hcygxuhm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2vobgnydd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dmmjjqjj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2cabozqdn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qasdwvyj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qougzduy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2odmpvmsx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2evesgcnm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2musuxfoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvyojtuz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ybiexwzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2keeotpdg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2lkuauycr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ntxyzqua.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2spzyvsxy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2uwkktrfa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qszowfwx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2oxplgcsn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xptejqdh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rbtfalmo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nksqtpvu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oobzebyq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2covcybpt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zngqhrxe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2jqwjczxu.html

);
来源：http://www.52xcode.cn/Article/details/gt2afbylrlt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cbbvuwus.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2slrexxho.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2zjjxtrsg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2teedhvmz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2gzngmmbp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2wqdvxzmu.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lbludwho.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2iffvconh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2olxoojlr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2pwzfhpqx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2tveyigba.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vmxadrup.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ijuyrseh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ytpgzfla.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mumlxstn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xwrpenfp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xifkaxzy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lisgsxhl.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2meebduqc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2nckgoaqg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2iribeimc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2prpcutzx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ahyvmrjg.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2yjbtqzlh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2tignduhd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2unmwcugc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2mvvecsrp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rpyidvgk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gxlcqoql.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hospxrae.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ancqisfn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wulzcivq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xexcvmif.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wewtcjoy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zjbodixw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2czwuluti.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zfgoyzeo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tkvqjgew.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2sohmhqbr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2jfqjykha.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2twbovxth.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2qzjqrtwd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2iffglxtd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cnlrmflc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2iwdckxgg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2snjklpvi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2stzknxom.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2fnunmidw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rvgwomvv.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhddkdib.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2yphdikwp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qyfhepec.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2bieavkhk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kutrzvar.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pdpsgaor.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zqumvuwc.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kffoveds.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wokgduoq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wwiulqtm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vopapqfc.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sdcvjhoj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2beqykprv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ehkrtysg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2arydbypb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zzorsbim.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dpmdxgva.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ibupvbuf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2epliqcxf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wgkftlhv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2mrydbfxn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ouapsjhn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2smcvrpva.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sawciina.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nhnmzozd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yssloyiq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2eobufrxl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2whrvynco.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2eazswamt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2dwzcgean.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kozpjmpn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2uuclyeqa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2xgegltnt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2thosnmmi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2dwnmjzac.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hvnhnapo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2byaqtsib.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dibmkaev.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2krhytizt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qfsxwocp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2trhutfsr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2sbwchtzn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fmznhmny.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2xtxmnkhp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ojsitvuu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qpamnbol.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vbwfyqop.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bmzszsva.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2uxloqokh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2pqeoamfe.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2odkplaaj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2veirdrxg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dmwltagk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2mqtclnsi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ugfqqppn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xtswznxr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ewjediak.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gmmqdhjn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2iqwfdlbi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2psjvqsjc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jjfvxgun.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2cmrgaktz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wienrtpk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2rcgwujij.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zjvkfpdu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2axpluewk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ypfdqrxt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ghmmvkhr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ebofzjwy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2fsazopxp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adzuvekc.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2geommkoo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kmtkvxhz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xegaxnaf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sbvrgact.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cozicfgc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dlagonww.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vkebybwt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fncivrvs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jptuvvfh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2npufkwba.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yndtbhhu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2uusnbnyu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ousmdmax.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2awgnfcro.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2oxcwafpu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2uhphiefz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2clrxqfry.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rbibbvin.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2bdabgexz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rwgwcwbp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ulujvvzk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yfiftqyj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lirfcakv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qywxklsk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xxoztzzh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cugnysjk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bcsejoga.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2nvubcwnh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wtfukgwx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vxnucsfw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xwcmmcmm.html


<!-- 参考信息 -->