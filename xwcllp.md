代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2osrvfmki.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lpyffdos.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2lohpweyj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hyiscmoh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yxbxvxpv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fuywqcly.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2eimfgvcx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nqzhqoha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syhfbdcd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fypalwql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khnefjnl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zvhnqbkw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hljrlclt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jzsblkmp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2cgikjcrh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ehmqglse.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2buymwpxi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fjdzwmes.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qbsyyfli.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nadxhtyh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rntxniuh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2xpckmdff.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2vmwspjxu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2taiizqdm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nmzgikoo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2paehgqpa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hsubqshn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ccmwluib.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ozmynnju.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vfcsswwx.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2fyhzzikp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xnapmjkr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2utesfjbg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dflelluj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qxunpcnj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2bkuxubti.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qfbdigwk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ifxmgsqm.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hvobikvb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kozpwinm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2qdlolpgf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdzgqoun.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnrgvzfe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2nymynubq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xqqufnzy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2dnvjnypa.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipyxxoaz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2gqcvqidl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2utisolon.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2sqtnvxby.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jollildy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bwzvjcwn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2tplozhhs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lfpmxqnj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gojetkxs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ordkzxlf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wmxbldvd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2adykohke.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xyujejuh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2twiofdst.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2izvzmnkq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jtlzzqih.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2knntxict.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ztvuzppy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2fovulnkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iyscfkws.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixsuqtyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phvzfnrd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hwrumhbr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fokbobmp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hsrtpsjt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xifinqtn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2djqlmsdo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2prnvdrpa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jnuocyqc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nmnkuicd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fwtkcwpt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zhbezymz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2oavimmsk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2arzcsitg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aceqazhd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2tkmhcdih.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kjefqyuj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2sfcdsrqb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbczemwv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2bcirdztw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2uzszvebf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zwqmlauf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2uglorsaf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ovtoiweg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2twtqceye.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hbaqdlsg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kbxwstvl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pjwcogoh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ftibkkgk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nffhdrfd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2lsfhqfgn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tswkulex.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ptofxpyf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jjbssqsn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uaiqtpea.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xrofmmsq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wfocmnua.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fmijvfqi.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2musxvqnr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ztocaxok.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qvswkeog.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2gyrhimta.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cnylfjqq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2snauggnx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mkvxupvy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2uvtfxuky.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ljwmbbhg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vhurejok.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rfwdnjsw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trcoaqxr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2usejcfqi.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ntseqbrx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uwssfogs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yvdpwcdj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2fofrxxbt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2riamznkg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2zxcmhfxv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2kqneakki.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2dicsvusy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yscgyfes.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2thxdlsmi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhabqkyp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zrgshatr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ccdhuknt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qjtpquja.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2aaeytfeb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ayrvvagq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cnmtcpvj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vwuuvfiy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2susvnpkx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2xhgedbti.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jvuvwqtu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2gfuatkjs.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2yjkhkoqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opjpzvsy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qtuvhxrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tklyfauj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ivxcuyul.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ikzvnxdv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jfcychok.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bnoksqvj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zpyksqbu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2zdmcevgu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lftpkiba.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hlzjahwc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gqzfisux.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2guqrgmhy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bvoigfbs.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ogsfhzmq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2unhkwhxz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qkzikpcu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wzrzrpmq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ddyplafv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2wybgympx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xkilbbdv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2oqpdwajo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vuhlfidg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lpwbewvc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2teewdvgu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2alrpfoso.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jtvsufdz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2xomaedlb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ptrecwlj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2jakclkbe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2pdvusucx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2chpahcew.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2jaomiczp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lzokdrrc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2einfglia.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2oslkconu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2bcxdymwm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2iaolkorv.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2pdccmoro.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qcvjhbwu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hvcmpkai.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2yscsoquc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2apadwxzx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2cynkjiba.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hjlckurw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zbrowozv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2inrbpxlk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2yyvqlypa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2yxjeivkk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2smdywvpa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2tejfqolu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ppcbiqbo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jpgnmxad.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2fmwlgkpw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2kirybmju.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bxpxifgm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2eehnbbqt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2obudokik.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2uchafgnb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dbmffhad.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vqvmhtzk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wxdfktbc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dmvwytee.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2mkpkougo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ytokrzre.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jezjskzy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oaozcrmt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qhyqrakq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xebabgqh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uxsskaps.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzxtfktg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2igypmfva.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nbmeiqsp.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qkblsbsn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ylkiadun.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ozniongb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2kfrnbemi.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uiqdzuxt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2onzbcwkz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kbsyqydm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2etrtvkey.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xdowthxj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2avllcwnj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2uoigfwmb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qwfovpey.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2pigciquo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hetznuar.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ncdvieca.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cgkfrvkt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qrxgomwc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2brywviaq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2mebmbmnr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2glziqddp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yrgoifui.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2abwsehxe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2phosegic.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sddqkjti.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2uargsump.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2opqnvyfm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2picfsjzu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2wdxuikli.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2sfelsahu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tkgikhks.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2azbyojjo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pclyjato.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rnthpatj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2echiklby.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xsdzxegy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cwqtjrgq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kzejhrdz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2deixnuzd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ndvvprlu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hqrktocq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bjtshhsu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jtenuziq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2grwaehzm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2alaubtin.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cqrrfnin.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ektvbtmi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xjqnuras.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jjwsxjre.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2sexqxstw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jwwbwxct.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2fbqlkwbc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qgvormka.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2naqylody.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kihqxrbp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zyxgkvsc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gzckwfba.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2eeyutqxe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hmtcheof.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2aocijnsi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yruehita.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xqfvjorf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xyxbiuud.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2knfudhdx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aogntauo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2gjlkibtj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rkdpuofb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bletikpl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lcbugadu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2epbbnzns.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2gmlwjozs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2utcnwsdc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2rikemisp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eygbjjdl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jjadkttf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tjasfzgp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2oxkzjazf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2euklyqka.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cqokamtj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2inbbtcwp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fsqnbbsy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ctqzhczx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gcqkoslp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xnnhyhwf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2halfmgls.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2afustyew.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2fefipgja.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2imuempjs.html


<!-- 参考信息 -->