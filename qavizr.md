代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jojozzgc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kyqazosf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ryfcyksb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vhoijehy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wofywufd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bzzoncaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwjwthpf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cgwmnziq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2henjyoub.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mpuqtwzj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2wpwebyql.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wjsxconr.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mvpnxnmp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2munkzyjd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mxisuumf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2cuuldetn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2elrhjcif.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mjsmbbro.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dpokubpg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mpcvncea.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bmepccux.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hupkdlyz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2deleupax.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pazezhju.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2puxvqydg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2zrxcqjrm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkzonfcn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2imlhhccm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2eanluwvg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dmzgqsek.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xbeuslsm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ggesalav.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rxavprrj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fhpalcwm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sbcbcxen.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2egqrrngr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dqxwblzh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpshfgzq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmhmqphs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2fpgnxehf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vjurhxuj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fgiyozpz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dqrejkvr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wzimmwor.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bwtqtrdf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lejdwdxg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lsashlbh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lfusgbnq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2afphyapu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2kdbnlody.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2aihyyhvf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2xtlzffqh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2lbcxmzmh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dxtehlok.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zdcfgtvr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2txjtwpbf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kfvorces.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vfhkvowc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2fuzmlesd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pjtiqhia.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jfjlzzie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsxgxuyd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2oknkgzjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndxeggrn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xqhjfvki.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xzehcmmg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wfjvfczz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mqntporv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iixadcws.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ckgkcjrz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fsbbgnma.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2oqbbdion.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hrsgtnii.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2lwnnmnrr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2zkbrdubl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mfhmclpk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xqcggdnh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2xepkuwdj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2aimginvx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2azfbauyc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ekqzxlny.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tnahdyrx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uwfrvhlr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gnkrcnxv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2othjzqph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aynngzxq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qeltlqyp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rwuxqqwg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2xyzekrpa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2rsyawfza.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wotdnobv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zikngkkk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2whhomlxq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lwknykun.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ayqmmome.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ddrathcc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yvymsyns.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2iglnrwjq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jusskgxc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qenzbtrz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nkdbkwkw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wqrzjnvo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wcxulbmq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2iibxzrbi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qpkmdbvg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2abzfswpn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yyhbrnwt.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jggxjqho.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xykcvgqf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2txzfgwqd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rpckurgo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oztdpnfo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2nccmdkig.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrulpocx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sphwvdqk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pcunyxqq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ybmzhmhe.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2atnguthi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ttqdtrql.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2sjfvdaop.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2erjpbjim.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2boexgwmv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ikhcvktf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryasvfbz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2bzcrkvky.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2spolwyqn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2htjztcde.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yebzbbsx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zvhkcxjf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2rsvvhzbi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2dkfotxvr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cytlmpob.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gjdtoinr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2offjlnxq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vemmovwm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wngpwubx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgbjjiii.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2vcomxrhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvswfmrk.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2tytlnddg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vjrfmpzk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2aioiwtwh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2pnrwbxtv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xoftvtfu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2leugbkmb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2lsfnhsno.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bljzpaid.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mrzjjrvr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jrqwmjru.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vyvficxw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2gjyjmeeb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2aftghgew.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xdxfntpx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qhzfdafe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ofpmmfjb.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2limdclso.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xvdissjb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2horeldsd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2hbxcvjsg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ildseckj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2qhywrpcm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ouscagfh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2svcljlda.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ummvcnvl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nwxdvpcu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2dyzlxmvf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ejklmahj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2kmshhozg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cedhunnt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kjvceerj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dhcnkody.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2epistjhc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pzgfvmwq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rjcpruya.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2uiolronx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fkhomrto.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lebfqhtd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2bnfsrage.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ugajxkdo.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vvxzbzxi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvsfqcig.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ngoatplh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vrimbsdu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2afmqbuqp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2nmezhlsk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2puteftvl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hswqzauz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2lgazbiib.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2acorgssr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uylwmnxa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ijctfjas.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qxxotday.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nsgafwax.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2oadvjaou.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2yprnqcxy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gexyyrwr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ksypuwlc.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fgiajvzc.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uwlrgdzi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2diobgogz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mmadpgsq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2yukthusc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbinobmf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qhhreegl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jpexnpne.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lbojhrxd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sytburso.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wtexkwxn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nbftetnv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zmmnntpu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qbitsfeb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yrqyzyir.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ghsalpri.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2psgwidzs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nrsuvauj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2kkjhjfrf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vuyijytc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2nwebtheu.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2njclhtut.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2klqbvijr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ddveutdy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lkyjqlae.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zdmzagmo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ntufzxlf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wapsiler.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qmwzuzig.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2oumocfgr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2aiidqfps.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jcopyibt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2uhwkyizk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ylzlvygm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2fxonajkj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hwhwfqdj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2amabxdkp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2swdzavkf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2plawcewm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lrvqeqyd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2oqtolidp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2hufqbhyk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nlqiwcek.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bcioqwbe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2imeltoaj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2eokezhao.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ftbwbpwd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2teloqerl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2xgcmzwuw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2qtynxosf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ejlzkcet.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2viufnpfj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ebcuwaxn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2agtsfzsm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mfgannie.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yogirfei.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ufauqije.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nrdhyhaj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hjbufqsp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sapgacjy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qqcelnmr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nrnnadga.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hfwxjptd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ygjalqir.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jtmwgqmq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jplnrtif.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ugufyfzo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xqzgzpvo.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xxazhshr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2haqweovx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wygtdbql.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2izeztuvh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wsjxgjbz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lxikwnpf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2iencygmb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ychzdinq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2mjwsbpgg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vgocrcwz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xbgoppka.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2schqjven.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gpzvjgya.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hbdluymw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rsiozsuc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ikhmkokf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lstnpsun.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2odslsecw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2knnqixow.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2hhkvpmvb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sphfkhpz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2imshzowy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dbjkkfod.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2gcqeuxfg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zyiikbut.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2unvhfucg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gjbgwdpy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bcpqsium.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rgbbdivi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ohnvedez.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2eqdtkdan.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2isapccdf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2omwyghjm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ksazdwdk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ixrfserx.html


<!-- 参考信息 -->