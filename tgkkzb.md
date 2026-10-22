代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2nfrrdyye.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hujlfphu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2szglpnkt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nalbgrpc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wsnhhdgj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzzofry.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2zbguftof.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rmpqlqtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxfaikse.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fhaprigt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fozgghay.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dtkekcze.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zrgfuenu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ojfhoxwj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tzavroaq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2imhdvxad.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lggazbrg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2gysgzbfv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yvcepsui.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2eplnqrxz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kxlcjxlx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xatgaodd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vewlozke.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cyrxyuek.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tuveecni.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2otlwyxoh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vtdxkdfw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tgpsfdkj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qotjfiau.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2diegmzzv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2nvlflbsi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vealurzy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2rrgtixtm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vtaybity.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2askhbbqv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fkhjknzq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uteemlcf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2twusrurp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ltytllba.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jjcwcpqj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jqwootdn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqrmqxei.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ioxqiwhd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2byrmbhqk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2lecrskht.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2meervpvf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2whodxwfh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2flynttga.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2udbfkawl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bxojgdel.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2awnedgsq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2sjjpiyyv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ncwscbim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2angrvscr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2xhorwcpk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mfrlbghi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vckggrvk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hyczytng.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2qzsdmqbz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bjrubuse.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fnnozpyy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kmafgeap.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xrkwhfqs.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lnwwilal.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ycrrties.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmbsrgyp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2nfhaaekv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tthpsjae.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2izcsovth.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gnmajbho.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2neylxgnx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tmjjkprh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2eobttaxg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cdmexapf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2kvpyofyk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tqzocqff.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2npnuditx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2alyfdkrb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qgikuoxc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tkpquyhx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2untokapu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2kamzuzcm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2loudptkm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2whezpewm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2shsyervb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2odfrvdgj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2glnkvswg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2tqigalst.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2whidojlo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xzzjhpmq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oqduqscn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2pxepkfjy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ogovpscw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wtnwtqeh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mesliwqr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mqsdypym.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2pksdownf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lmwcdijs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mukkljgk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kglbougq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ggbqihos.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwrcsmx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2acutpwmk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nhnzqygw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2pqbzeafd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2sqmnffxs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zhhdtmlj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2volnozjv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2aamqvpxb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2uonzmmpj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ftccpncx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2howwtuul.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kdjplgzg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2khtibwud.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bnrhkbqb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hsakmnxj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kugiviie.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnlajiix.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wysnfisk.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qspqexvy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xgcljyng.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2lyrcuiya.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2allgjxlc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ltwcaxnb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2kqhwpbwp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2khfnvlpd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rocxktdl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2kzcaaxbv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bpiupsuk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2iyetzned.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2epurxygd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mkhfpccg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zwkhmjpu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cbxjfwfk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2aajskkbj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fvympqfh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2idlccrpo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2oedieamo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2cetiqqrw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qewtlubz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwwvhhuw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2amsatwgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzjxtwgu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2hdxicqjh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zhwcuole.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yvcchuxf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wvntjqrz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2guexyshs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dtyfbggg.html

);
来源：http://www.52xcode.cn/Article/details/gt2rydgouhv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gpgjilgu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2sgliuulf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kypadcdc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2okhxbgme.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2oimriqqe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mxgynyyf.html

);
来源：http://www.52xcode.cn/Article/details/gt2koyyofbd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fczahqpe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gwvtyqcf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2jaruejiw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2yzlhpqxy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2ghneqnty.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2efnybxym.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ckhxtbnp.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mdyacluf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2pymmslnd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eprmnncm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2wsvedwpo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jmfvaftm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2cgfmtxso.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mcogjdjx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mmpmiqsw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fxgqckzu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nxsublwe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kpbvhobs.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ztpztias.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pclzqmtw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ntxcvkkr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zifymjev.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2irpyairn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xkmyazxs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dtlvmcnr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2drjjvbkw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2xxvztlov.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ejvptkpx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iyhtasfx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xyecvywy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qxoizpmv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vuallblc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nwfzoxwt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lhsurnvf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rryzlucr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hciwmeaf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kdrtzbmr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2rhzgptbj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jxrglwdg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2riujzoev.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2xqiocgic.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hfvimqlh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2dphsnbof.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2pmzcvprg.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bzcsynxx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yjgmulal.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bptxedte.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2didxnwob.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2eaqyvxne.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cuodfvvy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2usohclnq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kzjatfqk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fjacxnir.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uddyyark.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dbfijsez.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jrjyrfuj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2siyngskp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sgxuhcxp.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yhgzqydn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jqecssgk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wyopmcyp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wjnzzxiy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2pkgsdbqe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2zgetnsal.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ubeaskol.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2psyyznft.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wxfpfuhl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ypgwzajp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qajwefrk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2rziocuzm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ijuffguv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2tlwockxx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bdpugzwi.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2yzvpjozx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bypqyhby.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2nsfivzry.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2blzukspb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2rnnluicq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hoigdszu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fnjzeyra.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2bwwjuanh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2msvjnhyg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ghdakcsj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bsighhua.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qspzckla.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2uqgolwgp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2njuawpdh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2fnzbubpd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2botraeuw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zentmcrd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2pfynedyh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vmmbpybm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ilmphhba.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xwxipihq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hahayvqp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2zvrjebve.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cielwwnj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xwnxaxfa.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gfnzhydl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rotyiala.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2agcfxxnp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dsxodxfh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2duznnvwa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xywoqxao.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sgjaroyz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cpdefpqz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yrwatxac.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2txhqpvtk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pnmzgfly.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mbkolytj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pszxoxjs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2acqsqaux.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wpgwtwii.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2pnhfsrbs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hqjnimxc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rkbejuya.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ubrfmgdo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ogspxfhx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wkwqerru.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdngexmn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qpuaquhr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yeqqcuxu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ttcycdwb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qqsmuylh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yfcyrbmo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dvghtszl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rgprhjel.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2dshquncu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ogvjufjo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2cybxdztn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pyguojti.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2knksvljt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fqhgtrsu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2auggxgzh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mribsatl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2frpassos.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lihrdgmj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rxtdokse.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tmypiaip.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pehjnxsd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gepicpam.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xeannjhz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pxsefhwe.html


<!-- 参考信息 -->