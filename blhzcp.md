代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pxpwjgyb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2xrqattjx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ihllhvpl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wmegvzyd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kbjrgbxo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2eskslptx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2vjasavec.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vgpalsbh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fdqeoprp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qzpimnhp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kpcinnkr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2atxmrtcq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mwravdee.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vttqlgoy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eqeidjtl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2roqlxrqb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cucopixy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pudulkde.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zeliwslc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ctoyjeqh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2aolddfat.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzbuqotc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2twuolvzd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2akohxgqc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2oncgvysc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmhvbfxh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdvgijnm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uwypvfld.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ltvtpkag.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2drmgwsov.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgbsfkri.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2iuxsvrqo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yuoqlhca.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vnbetjhl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hayejhve.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pkuxyfew.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2talijiqa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ewvspmst.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pqecjaqp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2yyfjjxpq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zuipstas.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rizujnqp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2opvgyzok.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pmycnusm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qywtqait.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lsynlluj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2omxwgpvl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2hbzyihnh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nnwtmmva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhohbfkx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2srewqnoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnszcxgp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fawdgjfz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zmbunuki.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cemfcsyr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wflvpxsf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rzvllbmq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2aelhdnlo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oqnjeimg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2knxdpvlv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vtjlzzhz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dvlctquv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mxirynut.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wnfxrwjn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2acjyutug.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kdgrkjpy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvwxiht.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tvtprycz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wyihowhx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tpxvjwaq.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dknidnuo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zqtltswt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ehmkzvrt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2knuquovo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2njvuemve.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mjuvfxjl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2buvreeic.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ygucpbgy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2cuvnhglb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2lkloamcy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2drykcdsx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tqbfuzjf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mymhhvdg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tiodwntp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rpuhuiss.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2imhjgtsc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2qeveylxm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mrxrdlhk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2moijeanj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2dqcowmnn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2afsdwozb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2uxzedoki.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zozbpwah.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2zsjjtwmm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lxkfjtig.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2xncasoht.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ouemqdby.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kirgoodn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hxkbrwba.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxbhraxn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vfjwljvw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snsshdzd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2quinoqkt.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2bijlwxgm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nczmrjqd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rbqtbghs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2picgutto.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2onapvcot.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cvpxhaqy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vqvmzrre.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mmzzlrjs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2apaotule.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2qcfnngkh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jjrfyldq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jkymyxdj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2aozcygpc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lduzzcgx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2mkoocmwj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rxdfqfkr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldhhvycg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2uencdxaf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2dqntccnh.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ecakndfh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zciysixk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psatkyvp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2evcjzbed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2coxhffhb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xfojhxnf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2nzfglyan.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ynaczkuc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ouklulxq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2azcyirpe.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rzmgkvnc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rkatbzdt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2kkrzcbtn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ktokjysf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2aaupmudk.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tfppidvd.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2tnlhxfxq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2osraibvg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2imhtvuqm.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gqbxttxb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2nutjuvth.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2eqzgcgzz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2lfsiowmt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2qcdvvnvj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rjujulah.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wecorvio.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qjigizxa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hcrwxmom.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bkjslwbl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vdndtqxx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ayzmjfbj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2divhxmfo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ctfbpugm.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ffwpesxt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dldphhza.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hweifwog.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qejuuanp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kfwtmlbd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nrzvfqgv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2eibyjnpt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zmqyownp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2phnjipqz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2szrepcru.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bdqrsubi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jnukxmbq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jnosazhv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bflrsloo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tketwmrt.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2myvvopnl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fojgftbp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dsszirqk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ckqaruys.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2foubfkft.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2nlbhjqcb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2urqwnkjp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wstzoatu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nymbenmt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2thqtfizw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2eegzbtqk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qbnamziv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2fyrmvuid.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2uazwxlyx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ehjlvukn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lfsgxdoa.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tlrkxief.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2qiehvxza.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rczkrghd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fndfhghq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzkmvsft.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vjtqpgwk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2agyevwdb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wzqaqklh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qsedlhxy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ntiaqdgg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zldgatma.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2uelqelyx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2agolzyel.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vkvbogba.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qjftbfai.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cuwjwpau.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mociqcte.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2gehborqi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xehveupq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vhvsunnw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2btmsgomp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2pzwlxuna.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bjnbnvqp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zcjmquom.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qjwhujkq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rczvcvyk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2pymcaagn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pbirkdrg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xsuezfax.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gikiswvk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qzmydxgt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vbsraibo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2yiqvuapy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yviuyqlq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2allqsjvo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2fjbdzyyg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2gngmvtii.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dxsucddm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2elzcfeds.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2uauhffjr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2akkrrbwi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jmriwway.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tjhmhzrk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lmdxkxao.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pnherglb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xbjxommi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2euponxtb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2grktwmzq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2humfpapi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ddsyyxcl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2sxwwlvyn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sspvnjrh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xreyyety.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2spweqpxo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tombxfvz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wnbmnmts.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lhxfsnzh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pawmxdem.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vfetkdem.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2zdiweqxf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2spdbuwbt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2thprxupo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2sbwtszrj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2vgbwxhok.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hgpvrmje.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2myrcbktd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ymggdzwo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dfcqawrc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2obaglsgg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jhrxmzyw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lvnexlga.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qkurjpee.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qekevgpm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dswxxpuo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urvfgeky.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2mbwxbhbm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2keijjpdk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nqixtxtq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lblaamjb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cgqjfxqp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2erlradfe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2warbbvha.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2auifyyvx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2reqbrrtw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dxhdegpn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iqmcowon.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2abzoiofo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2nnetzdxs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dpofgdmd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mdjwhchs.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dmvmxelv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2yticepcc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fpkmbkui.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wkpzqiss.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2gufjkgzv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2chgorgbe.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fsjvaheg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2beozuogm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2suwqprjq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mysoxcpr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xofuyofq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2eydngcwl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xzpgkjvq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2oufvgjoi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2heckuysy.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xmipwjmw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zwceuggo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wskcozxo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2xyokshrj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dbxtxrnz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zdvqwlrs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2survnzjg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oqsvekbb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vuquskvt.html


<!-- 参考信息 -->