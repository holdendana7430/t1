代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhauqzzp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xnoxhdss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhzutlbt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3yrifgunz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wvdfdedu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uhhpzvax.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tdvzolcs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sotuzxsx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nxinhojl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3itfuvtfg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jnboayxq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3iqyhyrro.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3oxxdwifk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ngyminai.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3jxxjdswq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ffpvbfjq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hykwcahn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ecjnistz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3oelbektf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3dmlrwbpz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ymikayhu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kkwyvbbd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bxhavkbc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3sgfiqcdr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3bqamkckq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wjfkmgad.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzbdmium.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mwqiieqd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqcrovu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3puzqqvhr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lxjxynlh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ecufuulk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3nrhvzxeu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnwdmrui.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fokwrtvx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gdvufkjl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3tozlaffe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3bqzrnent.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rogibovc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kdqtuobp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3achrxpbz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lmxichhf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ukleelqj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mwqyupjt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3lboqeuaz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3oiljihaz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tabqslci.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3byygaxao.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3laoajzcv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3fotcfqet.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3kdktjdom.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fzigkcvn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3mcmhlyog.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fubdchph.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rhaqtifw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hmbvxbov.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3xxjgglun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgeblikm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3lhmyftfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qskxtyeq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nbyxszxd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wkctfifu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3flgngsie.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sizuvsoy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dwhigdwo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ohsymvwy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3votaxpis.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3mnpcsulw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vxsnpmnl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kmqhrtfh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3izapgaxn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3farcrhsb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3zdxafmqm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hxpxpqba.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cihkvdop.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wffffsit.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wkntlugx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3btaagtjz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hjyprgwy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yvjtbarq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ofnyhftf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wdxjenrw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vjeigfpq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ssnpjddh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wqjnsbpk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uhhjfcef.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3qnzwkgnd.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xohlijmv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3blqrghki.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lxijkaxk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3efrdfrus.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xjweffcd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gadbwdnq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3pzudablh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3qwyvrhtf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tprinefx.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3yfchymhj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cllubsib.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3qybrypdp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kdqhsvcj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3waygadil.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3sqhvbfdi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sewecgnx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wtpdtqpg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jzfykhns.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gdpjpgiw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3miekguvi.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqmvikza.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ifjtfzjx.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vsfeciud.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atevyyyu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3dvkaqhyk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3qsvpmjpk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svehbzet.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3sdngfdij.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3adfwcnbe.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3oktgcxhe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tdtvqmxg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dnbrotzu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmsfittw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kwqbsqff.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zetcpjpa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3opkpbcuk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3tnvupqzk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3lkjvmanc.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ivmiiwvy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bsodtkcc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xcuqhpvu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xsdpsymy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3junqontk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lgkktlyh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3lmeqxgio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3porshhig.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lhresszu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwtldlzb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3twgzjiep.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ploctwya.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3espdsvzk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3erhabnnr.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3diovwiok.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3thjsruhy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tihtvnrt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kwkhknwv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3idfusrmp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3khnenkxr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jsqqydsw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3akysxksb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jaiqmbho.html

);
来源：http://www.52xcode.cn/Article/details/gt3moornnvq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3bpokcrgv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mdmltnwp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3youklafn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ukxvimiz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3etwyihfl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3aiarvgso.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rvxcsqxd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3efsjuzju.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bkonafgq.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3hfguybbs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3irvcguls.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3qetasvzq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3hoieiymo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xflzlfkj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tyvqnuez.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rhkmwriu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3rebzwvcf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hmihmuff.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3psswgwpu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qoksiaag.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3foupgszn.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3acyvscbx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uftdhzqv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3dtbbvegn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ntpcallj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3escbwelt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3adtjllts.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wxpyvtao.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ixeuhkor.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fkqankjy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3lqrgtwjs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjruqhau.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cubhrhmv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3igawkbbx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3gioxcipp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wpwfutih.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3iuhwmmjo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zbxsvpjv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3uxaqgavh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3vgbcuejy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3nvotjery.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3rvhtmhsp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3mnqtoppv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3opcqjsrp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oxakpuie.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3piphcgar.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gvyiajxb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xkmnkvwc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wxjnjxik.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3knhsqwvk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3urtqtfwx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ghzyoezj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qixmhkmf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3duryuewu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jsgemddz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dvfoctxs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3iyginzwu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wljhkgru.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3loqblkon.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3jenwsrhn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vmaatelg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ywvoqsif.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3vsqxlrrq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3uqichnze.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rynruarm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sxnpiaoa.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vwlzgbtc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tghznirz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rqhygtsr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xppqxnym.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wyjpgnpz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3qmwgzydm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jwzqmgbn.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3trcwfvcm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ixfkqlov.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jtcsrxyl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bssikukk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tecgeiak.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3nbrmbbdu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3igthwezn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mzydnnrw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vflactxv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3lodtrcyf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xlbtymfs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pjzhpuhx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3blscqsek.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3fwdasfme.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3foemtcyc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kuaxbeor.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3chwwytsb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3eatspedl.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3scuwnwlm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kucrwzpq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3msqukmov.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3otcpayji.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3lyxrjwjj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3tvibwqqz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cecwlrrl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3azgawchq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wxavfhwv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3rqvtkbtp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3hjrqsqoc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3guvpwdqq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rauhtubp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3zwzxdbsc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3aimpfeye.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zmafbtya.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ullbqgvu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wctknyuo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pmjdilgj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zfthrrtr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dhlegium.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jbsnjlhy.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3kekfsiac.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nwahqqql.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pewilnoo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3plfvybhh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gagizynt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lhnjppep.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3scegxhlz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3pwkrzhjo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ptkweutv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hsmjgrhf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vrhhtacf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rglogrco.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3jarciztv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cucshpxg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3tzloheah.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dplystcb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3pknnfsxw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3srzwhvsc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ndjqynzd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cduomjlm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xleuxowj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3szasrmyf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3djxxjsqv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xqvpsnfv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3nmffzhhi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jwywnghh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3idvltujw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hquyrqdz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3chmjgrda.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qsozoteq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jxhnhnmm.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3aemufewx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3blrukomg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3bvaontze.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qarckhhk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ofqnejlv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dodcvhbo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vhhuhklw.html


<!-- 参考信息 -->