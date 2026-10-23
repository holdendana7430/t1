代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aitxcnby.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3clqeowsx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ilxlbcep.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3acbjuwkl.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wchhqnpt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3afzvqywa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ftlzixfl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ozfacvvv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wugjkxdl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ronkxuih.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3hkjwzkko.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3jgmdqgsp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lmiehwiw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vnbdjkwc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jsupyvfp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3hoslpdqr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vmhuvvjj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xgvzivcu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzedinjb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3gqnswomr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wnaoeqjv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ivgebyvl.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3huhezkoq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3juilbzkz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3qutsaksd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ulibaaef.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3iaflxlpn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3vsesxbkz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ovfhessi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qzoxpnoq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3heaapxfn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kuoyayrk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3xrtmbtbe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3twwumoag.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zvicmmrj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lbyrwekq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3xfptzbah.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ieacmjct.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3inshskmu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tbcrzbuw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3miyrnzzp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cvubusqc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3dobihtgf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bjfecbya.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mbyjoort.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3svafjfpi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vlecabyg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3fwqpqmxl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3qfymboeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulapjjra.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3kismzbkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttirrixh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3naktpijq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wcedlglw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ohvlahyy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tsgdecmm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uuacdeth.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aypbzdnp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3smhawuds.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sccrnvvi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kltkpjgz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3qpiswzkh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3txlsgicy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3kffgihxp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pojifdsq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cpnwnvyu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hruddwca.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3slmfcuro.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3eaquytmn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3sznlsqzf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rxyfeehm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3koghpbvo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3woftoawp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ugbjxlpu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hfsklntb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zlspsfcy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xexdwogg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xlavggaj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3npyzmsip.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3bbledqgn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rzdbvpmt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wyipgwgm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gmahmhtn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fmquoaob.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kvrmsqei.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mypcmvwe.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rbsiwfcl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uaetquru.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ftnbjlbk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wyqbiyru.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vafkzmps.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3nnhmtdsl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xnvvnism.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3zhnqwhkt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aybjnvea.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xdhiijdj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fuiwqati.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dqswylmz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3fqgaiavz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elkprbsl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3jhdjtnuz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlocxjaq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfyycsiz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zayddnfw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3oxzuxojz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umqcuvok.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3unpdcdyc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tsvyjgxs.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3odmiaibn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3admgtnjw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kdcskcus.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnhcsjvw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3oplinmck.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zhkblueu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3gbvbhscq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wxsmkcum.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3clzntxuc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pbsainhe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tvfnaeju.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3czfgxdsa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3dhljdqxk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3cktqkoeb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lxkffrpt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3vsrumgaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cljhjfjx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3flriyydr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwanbcpo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3pixstnnv.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dbxhzzqp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3oaupflbb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vcafitrl.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xingriom.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bhyzbsjh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vvtsnofa.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ejwmhvfk.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3nfkwhuoo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3coewabft.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zcsmpvnp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pppylbrl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdolcfl.html

);
来源：http://www.52xcode.cn/Article/details/gt3fixteiid.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tnvtsfei.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dpwttone.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3qhcavtzn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3imwicbcg.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jmfvwstb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dphnmezp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wtbxzfyr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3kxktuktx.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gakoyaxx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3umztijku.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3xaoqcwjp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bqqkbmzd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3rzmybzlu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3izhnpmdy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3wyubnixa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jufdvwuc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qsrqfkxq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yqcxeyhp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3umntytbg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3zeiuxrin.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3lifxvdlz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3demizhmz.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3byfxirlf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3xrpqikto.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jizfbzhl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jwmmeslf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3pqtximzq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yjeizxzu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3pdhkjlpk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sxhlegwj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3utneaved.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lqtmxwhf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bfwtzgfk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nxblhwvd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3udubcppq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xelskokw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eojtbirj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3iqyodljx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zijwblci.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wqwlaako.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hxqclojg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zdsfdqgs.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3iwlhudda.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3skvqihju.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wvlfaait.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmlxbylf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3aetgkcrj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zprjzqos.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cyzhfyoa.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3srxgepsi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pdiqkvpm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jyhjwfod.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3nhyovcwr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gusheukf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3txjzklwp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qsjtiiaj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3pkmjjrge.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3abnmhnld.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sfmdleqh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gndbyitj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwowdqoq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kifwfdxj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3pjbakdgk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3mwkphpmz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wvexvzxf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pttpozqm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3qmitnoed.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3pkjfdeyc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3imdtzftc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3gjfuvscd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3upcxtwnt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rbweyvmc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zwycvfbe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3zxavsnqq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ulpvdqnx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3sgnkttph.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wknlqima.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dxxsvjva.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nmcodyqt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3yjzphixx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3vchmxevt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3swfszfix.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ggnxpfzs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ejxbkwdc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hwjwfdmq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3emzjkrkl.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fwhmmgmz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wvrbjgvr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3phwkpogl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3cpfyyqfq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mwrsvqgh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3rlhhkmct.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qiezyecf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nweurkiy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3cdzklmgg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3zyapqrhl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3dcfstfzo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3qfhidgtb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3xdoflhuf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qidtmjjf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hlzxikbb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hdqlnmxx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3oxxsinkm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tvnwxxhl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qdxwyjmx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vvvjtpun.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ovsttkff.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tlezbqdb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3edvzizmp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eacupcro.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jjjvklgt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jujzpifk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gjhcurko.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3mqrgojyh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3ckucjonl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yzishkqz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3uiwedibi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xmtggqae.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ijhziddp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxhlaska.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xzmkarpw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hzydzbyg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3jyjqkuvr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sfttttmp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3hwpmbjvz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gwqtppwa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kuqdxaea.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3btflrtop.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3usfpljvn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3udmgvmjq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zkufdxbj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hbrsvppb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3dnievlvz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lnczryza.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3jbtccdcw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gvgrjmrx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3beubtztr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3klacsbuf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3sjyrfqsi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3seckttbt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bhylmhdw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3glqgrkvz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3lcdplujx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qvbdymke.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3agqegtmk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3cosqkwpd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3dwapaaxu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dsklbzgt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gbkavvyp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xofrevar.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fpfcdlhc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ihxbmqqg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3kaicpuxp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gqnuzrpl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ywxiklzm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ngutgqec.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wiacndcq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3txhoxopt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ceaugvbs.html


<!-- 参考信息 -->