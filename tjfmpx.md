代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctdeapio.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3oubjvdqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zuqbsyik.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qkkyognh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3iueqlxji.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3txfsmblg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qmqyfjml.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mxxggkck.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aruccpuo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zxvnhrfo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gquemdkc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3dnrvkwcs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qicneldc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xoqbgnye.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3whsbzcjr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3koeqeqty.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yvpdpnfa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3tivmsdvy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xwbhidfd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cqrjezfu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jcmdjqun.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fhxadmjw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jvdjohcn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vykvemdw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3clhabrjb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3erqqzrbb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezqqkecl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3veyaumid.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3oxoxqcem.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rzsogheh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3zfnuawzv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3dpkrcdpv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ptwjutwk.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3yhhfywfw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbxtampf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3krvkszly.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ekcfceel.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kefpileu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3gqqvkkad.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3uuclcmip.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hcqxwrsl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uxvbhemz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3goxnsixt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3joxjrmsd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3wvupmyli.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xxqgjazf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3spekopwa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjgkawin.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3krmvhpax.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3kjcutwld.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3qvkhpkge.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yrbpwwuz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tdfmdcds.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3chaaprob.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3lcoqsfad.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uiehhjwr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kdlgmefo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igpjuryb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ilnhozxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heahiqtc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3czfsjymz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vidyrcec.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oqwdbslj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3imetqpox.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3maxqggof.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nntkyxlz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vwkwuazh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gwaqjdnq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3obzfxoux.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3lcywyqnc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xkrvhelq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oprovbhy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3siogyrum.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bapnczoo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dxwxxsgn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qjrnchnl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bpembioo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3ucyvjilm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3irxwklwl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3xskmzpfl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3vajrlbrr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xnefxxif.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hwmgfoav.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3uiolkkma.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3txhpxvut.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzxvyff.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3clcybzrd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nbkztzoy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3voqpjkmg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3riudsxbs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bmfrqjjc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3nhqrhajt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fmxosrhn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3dqkgrnag.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ywydxljq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kykamltq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cffghnrw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tioagrkw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3cmsyzulz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3srgqsbwx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hypdekck.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3drpplzzt.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lrfdyvmp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ridjmkwo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3xcgsibdj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rbxzhnxy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eucigxck.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yuxppdbk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dmdhofmr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djvkdvdp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3okwoqfmc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzriiaui.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3csdhgazo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twhvtwvc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3isibpzfz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jnjpukaq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3aonlczku.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mtptdmwz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ahjynrhr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwikdcqb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3eqqskynj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3czupddzl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tqpjsoss.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jwehhqny.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vmprklma.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yjydfmfq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hwfyvaqk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jgehoomc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lzequqhw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jevakket.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3pnioleib.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3pjcteqfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkrpxsbg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nyacknqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nahhtlur.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ukzgiczw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lcvkgxzp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ceummrlq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3akjqtiae.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ovovptbw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mylwgeug.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3eueunmrl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gjpqzomg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vlgqceyp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rftknggv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ccevhtzu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3lgqeguhq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ouwojnum.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jmweovfa.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3mgihrguq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3suqqwbqc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gkyshsos.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cacdlyef.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3wpuxbwot.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3auowtbvf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3oxedwliv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ryjxkdum.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3dlerzdzn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3fpadgrjc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3obzaxpal.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3plqdvmew.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3gqpumnpw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tomklwfo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ljvbgwbv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3upbvobez.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3evjyvzuw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3euldxnnx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3laptwjrq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3empwsgep.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rnaooevk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3kjpcwouv.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wwguzjgf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fstbyjmg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3guhcfxot.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3orobvdwi.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3zvicgncl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tvctwtyd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ovxfpzmw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3canwrbze.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3secxyatc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gymbshuv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fgqgspsf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3lsnazyqu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3zdjfjhgm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3sthmmgmv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ogclxqkj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xeoidiig.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ackzknhb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3eoedvxuc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3cvcgqidj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3aqivclap.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ghcqemjw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3izeujoap.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3utoqvrnz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qgkqeyrn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ynawzqnn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3oytxjvoc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xlenpeiw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eybqagqt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3sytdpkta.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkzefvpa.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3psyadpji.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tzoqpavf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kwsibmig.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sadhvguy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3sewrwoki.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bxjxfczo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3oqsynfbq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3uhuvnvbz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tkqblnhc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ibrwdxcj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hnxoxdig.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wgbbabob.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3walndtia.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pcltbttk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jowmkofu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ivafljcx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ypbotnsa.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hdrsyszk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pzgmvfbs.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hzolslri.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sbsccexi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3iyhmifzq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jfekwvpq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3dewcywvf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lgxrchyp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wpjeixvp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3btcoyeat.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3jgqblcvt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ojjktlfa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3wtqcygtr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ubvyajrk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ntriguyc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nydlelyc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3dbmrnmzu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3tkbtpsxp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3yetinzvo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3hzocqkft.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fmpknwrl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3likjruzo.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xkumfbmj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fggwocso.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3zkagvwqa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3shfcwqfj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3syhdiuxx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jzjlvfke.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3osgjgcxq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3eowyztek.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kblayuxd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ncuyucif.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gwcanolb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mpivrihz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wyzsoovn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3lxthoooh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ftgxqhgp.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3jclapogw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3difhsdvw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ykowbfuh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3othpsanh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3vtqtkdlr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bwpuxpkz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3soonubmp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rltxiawa.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jklwstyk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3mgyplcpk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xuxyeixp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gonypqgm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ozjrtlwj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wndmfptv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3nfsvmxco.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gkotgria.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cddftlje.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ovnfksqu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dqfcqffn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3rwnppjkx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fhtaufab.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ftqlppus.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3azqjgiqy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3mafklerk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3gdliqcad.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3noiozylk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3tofsphtp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3oljneztw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3qnlfycpt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pyofchgi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3dqackulv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3chwbmath.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kiolzhvc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3kwcnpmlj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3yavttfqc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ikzvugmj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3myqjkjrx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iqmqbaur.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3etrgzxue.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3oobplbhw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3iqvkhocg.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fhofdpmd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3itivwnbn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pdbavcmy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3agtkxjij.html


<!-- 参考信息 -->