代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zdrgsjri.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3dskrecxt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ycvzlyqz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kjxelabj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cddbasos.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3huwervrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqnbynnu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3letkxvvb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sesmvahy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vxsvdwcb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3msupwoos.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3byrwrovt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kndludtz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bumlplio.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3irirsyns.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ioampmdg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pykwxbkp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3htuvwucu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3izqbkzej.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kibkcgip.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vtiinjwh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ywdqktye.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3otrlyzhl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3owksnuqg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3qpdzynbu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3gtklsfho.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wafnyzop.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gogtboim.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ccfggtsw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ibhzfjxz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3epaajumo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3momettbx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3fdyalvmv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwtmtfqd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yyjxocgi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3apqikuhw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ghvtfkaf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqsorfds.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jesmfqob.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xvzrbfig.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ovaurqdr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3heonjiut.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3bxmyblmn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3elfwakbz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3epkmpswm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3owoawdgl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qhilkryi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jedvmaqi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qtdmhqfm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mpzupqlx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hnvqpbgm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfcwofkd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cojejbts.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ycvvnjty.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ueyhpdxs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kpzimwiy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kfhcxbvt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eoennfaz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xouryjkr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ryhrjxop.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mkuszxfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwnhlajz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3kuziubtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfkiboek.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3oiczmgjj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yzpguqra.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fhacjsgv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yfjvqliq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kjnumxep.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kegodvcg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ccxnixjd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ruxewisj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3afkexpha.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zmrtqdyg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3udfnrkhu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pvaqyrjt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vtipcela.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3eacmqbej.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fvgllxtq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ylaoyhsa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnitldih.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rzaaddrx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bqljephb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kpbqtqup.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3egrgphgv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sdjsiblp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pdpumisi.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ywyztokf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kylpxgbd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ceopteop.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qwrfumaz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3nqtvmgjb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3bevhvfci.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3huvszuep.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tlefxhkw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gfweditk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yppwzsdm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3njrkiwli.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3askdiclj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fifzebzp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3scdexazr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3aocjcmlx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3sqmntrvl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oyjrxmma.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pvrfcxvj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3hvfembeb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbssimx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3icqesjrl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fcmkwimm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3lpebeqyl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eknrayjn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skynqcxb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3kgyzqrer.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gamwohfl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gifgiybo.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3lekmtphb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3kdwzidtl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcygpbcd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ukmosyfn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ubiwppxz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3bgctcgdd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jdojjjxp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3knitltra.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nidjvsge.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3fownqubh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cslzlxkb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3svzidznh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3yewkcjzj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3juaefile.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3zczfecxm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3pnjdtrfg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qwshemkx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3qyfcbegl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hsaoqxaz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ifvjdqow.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3npzllimv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qesksest.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ugtgnrdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oimdyemj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cdqewaaz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jyobrxuw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3sghndbbr.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nzhkjpxm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3btdlztid.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qlwzgwor.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3knidibvl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3snsrvgqa.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fncocmon.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xoupyljc.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3sfauxjyc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nhmpphil.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jwfilbvn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3evxmdork.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cunmnluc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fmlpeirq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3paxtjdyo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xzgdndph.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ulptchkn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mufuwwjs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3gmbaynqb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3wegkadff.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wpypbvjr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gzwdrzrv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3qvdmdjlk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3odlwytim.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3gligcokx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3iqqyazux.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3egczlasu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3epahfyue.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3csiazdtl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xkoyyaai.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3nmfndzcy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ghtgnmcw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3qenrnaca.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3hbivnmuh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qtyrfjcr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3upfwllkk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rffrqptu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3iqmgsgbx.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3zphisdzs.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ichkvobj.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xygtndfu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rfiucggp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3mgerrfxi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3icclefis.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qtnbscod.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3czqrjivl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cwmpitci.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ozlajwvp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hnpyylga.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vtlteces.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mjkbrrav.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ipvziliz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3pmsmknat.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ehubnigo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3czhcxvgv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3gsxbvlxh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lkkbkpfc.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nsufxkpy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3litiqvgn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3owrirfee.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ftsvbaxr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljawpnso.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pcniullt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hxizglas.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vunhkczn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mdwbgwyz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jnqrisym.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wphadgau.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3twxjoyhc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jrsatcae.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gzdfvmme.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ekxzqjco.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kbwuwulk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qdvkgzxl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3elqaxoya.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3twjikhfi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3lkazgykm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3orqjkuyd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ynkqpgkw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3oeaatxyl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3chrxhmwk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3aqqvymhf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fqsdedzo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jzuqnyix.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yqltomyy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tidmjwhh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lllwpkip.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3mpkrphvp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gxttaxfw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hfbavnfc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3lfuvarar.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3esjvgbbv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3anflcxve.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3unqylfsl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3bbbnmehm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3gaowjvaj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ghlizsce.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nnvbohqv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xfbjqopf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3enckjgmw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oqcjmbkm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bhubukar.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lywgtcfb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gpbkyuvn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ocgcmfet.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3aficsvtm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fszzcrin.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3tribsaps.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cwvmexkr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3wnudynld.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ppldlclt.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3toquztuy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rfkjvsre.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rilyrayf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mnvzytek.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bplsgnsi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mkdvbfnr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3chzsgvln.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3msnpxilr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3akwtyyqp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qkhnhkyp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3feulviwl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3djwpxpwp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cbitgqnv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3equnlpgc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bxhrkcqg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vsedutbe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3uveetsar.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ppwxfqwa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sjvwtpde.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ytqahoer.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kuphxtua.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ufcnnlaj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yunjjvqd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zhhxdbnj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tgheluva.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3npfszeqz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3owcyqhsu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mzqqljiu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ysqzjpjz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ezrozzqe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3mzgigbja.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tznlwxal.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3szkpltmb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3cwtavvae.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3beyhonwh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ohsweqpn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3mlazpuxj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dyfjrucw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jblspgum.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3fxljfvoq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fltkqicy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3frymhhgf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3djmflpyz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3msakhnoz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iyxzewvo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rbgzjmej.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dcnqeawq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3nuzfzycn.html


<!-- 参考信息 -->