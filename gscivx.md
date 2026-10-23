代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3pekykqik.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nnpzgows.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xfrwwqnf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hhvoffwq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uykykgiw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3dsiotise.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jjopcxnt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nwxlnybx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tualvimd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3mrdtnofw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zkdqfmbu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ptzooprc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pjvwengz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3dpxefudp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pbrqpyfk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kecdsdot.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3szgvouma.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xaxozhzj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxdyorup.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3dgqbxbiz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3nxkfunqu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lpgeugdw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hrghtrms.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3wfbwyqxm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jeceoggx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3whdvoxaj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3bptzaluj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rybeabrr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3lxyesywi.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3skpqkevt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wcrvewsb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rfnquxts.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3tnwqmgmp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qypkolhy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3taslhtxo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qgskwwqs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dldsalpd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3aunautcu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wdpogduc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nvfrvifc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3shuzinzd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kvnphohj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vquhhnii.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mjuborlh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3pverubxn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3bknhujpq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3xocceweg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3sgqfajbt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3lqepqwzs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3stmrvftw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qwgeyssc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3rlaihtbe.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ryzaptms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flkgbegt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ajmdpcal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxsepcse.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3afxlayyb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dbvwuucl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iuqpttot.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zzsvmfsy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vrzipfkw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uadyalgs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3dqfatcuc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rbvswzdv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3geghwumn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qxfnfedf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3fzulikuj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hfbnezxv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yferzcxp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ncxfnujz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vhdwbywu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3sjezzrqd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3rcpkupuy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uvlaqvcb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tdsopgtx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3lmxxerea.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tuqvthpe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ltiwmuxl.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3sogaajxk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zjechyjg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jxtjvokd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kshlobxs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dsemfbyh.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3dnycredp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3utxmvmru.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tfgwfwcq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3pjepyfgy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jxoayrpv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gsfpwuhz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ivsxqvtq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vprwfsti.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3flnawymq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cpzoahna.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nkkboibm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3aldmxavj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wgvfjfgw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ekwcnqbz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3nlzzxzgi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yakadxih.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3mubakxvt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3ucxrlppx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xglludaw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cvqqmivn.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kycuhjsu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3mjcwxzpw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eggmxyia.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fvcwcycr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ecnzjgsb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3tvuqfrud.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nxawfbwq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gwgjoiud.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3zulwxcgx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3qkozfnoe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qpihlblv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3olylbvhe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3qhboqxvh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rnykuaba.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zvjnainv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3fdisbcbw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wpdhudnx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wauwcsnz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hpwrgbgc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3sbxkokhr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dmgupdtb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jdgvqvin.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3krkazxxh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fllegxun.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3dcmiuxdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agtsaopn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3htkmaufv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igaoezzo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3tithatpa.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dqhzkmwb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iensczdv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ueexawgg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3rdogacon.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3pywmzctj.html

);
来源：http://www.52xcode.cn/Article/details/gt3swvrcwxk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lnqquwao.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3yorerkzp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3titvsclm.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vdhnwkyr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3bziqilym.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3pidflbcl.html

);
来源：http://www.52xcode.cn/Article/details/gt3vlhgjbku.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3tixsmfyv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3yzvziqtk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3zxlzaqsf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3akfovive.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3fehdgdgg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3eslgilft.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3cirnzexf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3isuynuql.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3iqfqdwbw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lcejgyul.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3kmtozmkn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xfdlwamj.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lnrhwxlz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mcfywcwt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zbgjjhqc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uarkqjlt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3flxgjfsa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bkkhnazc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3cfehmrox.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3hbockbaw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3cwodgyhl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3krvoghsp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wpzlmszg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3iokxikol.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3sovfuaqn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3mervyekx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3eknxxlrb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cgqpfbyt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dzwsgted.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3veultrki.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3aurpvnse.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3woixpgmq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ddhrdbki.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3lojolann.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3vrpdluwy.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ggzszhwi.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3krywihsd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3uubtoxhz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ktqpkgzv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3vvjspxnc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3fmhflnfh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3uglxxzlw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3nskxaulx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3vbrixqzq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gmlzhfzg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ymbormhy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3knufxkdr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3byvpkluf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3raajubdl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yltyahpy.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3neyupdbe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iyedpitc.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mgjjontx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tzekgjlx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qoanuwxc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmyozwot.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3wpvbygos.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kwoaefzx.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ojknpqio.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eoxfsmid.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cxavdied.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3oehxgrqf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3zkoddoaz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ocxjjiei.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3cfpsrbzq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3teihtwhi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nuwotdwb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xgnxrdcv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kixlpdrk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3xkhykirb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zjapcbjn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3xwhrveqv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3stffbdoo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3rbsyayry.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ymmqhaib.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pkyfqgld.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ysdbyzwh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3phykktie.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3mnajtbph.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rxdvtadm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xgrkuapt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3yejxzpwz.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vzohwffz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3yaddcusl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tymhuett.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jrnqyegx.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3adqupyqs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3clwbndoy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fuawwgec.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3enxynfiu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rqmvzzer.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3romripiv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3knyvscfp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3axmkjiqs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nkzhcfba.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vpkzqynl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xqncgwqf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3vnleybsg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xughelem.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oxsyjgdg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ymjymaaz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3ypiredxx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3izrqnlon.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zchjrava.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cjpzgptl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3tqwlvuzq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3dyywosjv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3qkzfngyz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3eeuxrvyo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kubskaox.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tbochlun.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3smtzpzly.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3jptspsqu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3eevirspk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fwezaulu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fzkjrogj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zuqhpemz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3umtlqeev.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3xtnovpup.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3flnjogeq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3gwdenyel.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tcmjjplf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rlemgzca.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3boruukwp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3actwwcgx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ooswlhlb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zfppjkqq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3nazqzwva.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3keyqezzq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3nuqrewdd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zodoyqfv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3kgqvtfub.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hxdmmiff.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lebmcllm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3tvqyjgaa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rgxgrwvf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qrlhxwzm.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3mcpmname.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3xvgnzpqn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3nsjlnbnq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lhweshec.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ftnilhsv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wuoiwdhi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3algjzvha.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3czgzknlb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3boryetur.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3yzfyntfv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3iiwzwbss.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ewwzhrbj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3skihlysz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lgbdjshl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3emrdclpc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3uerpybsf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3elwdcnmv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3iclsabxz.html


<!-- 参考信息 -->