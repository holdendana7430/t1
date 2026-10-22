代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zunlaija.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xzoilrzd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qeizzvsv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hcseofey.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2eqmydnum.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pyqwcoqi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hayckxxw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bzygdimk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wpjegvdk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2utlsippl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gnnhsluy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vjymlapt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fimligcn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eikjwczv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fsqkbcok.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rjpnzzqm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2novxtkab.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2crkueinr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jnlcicfq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2nxzpyzxa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2byzjynsw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pdfggjdo.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncfqodlm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2fgjhnoty.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pykgkgvx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vseyjmwk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bghmmgpo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jozajdxv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ewvyhbcw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2soohtcfh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fnyvjwon.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2qqogpyfl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cixwfqdr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hlbmiblr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2tgzofjoe.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2zxmokuyj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2jigkdowz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2txcvnyju.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lduxzfvj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jamvmjlh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hwmssoek.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2mqrluftb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hysyzjbt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dojaoxgi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tpzavkcd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2rtmibcxq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ohozksvr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mubqsqxa.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mybsehct.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ybabfknl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2nfsmoylr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gbbfitas.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2slulbtio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klzkukuq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2hefuguwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvhwszia.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fdknqojv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ldywlwdv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wbwguhnt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2eppngths.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hkxghxvd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ndqzgiwi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mvbzkdnl.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sozycvve.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nglevoep.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2lhihepzw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2hvdfhsww.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxkxqiuc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mnpdffpm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2nbqjdsvp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qcmilxvj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rqgxiawp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuvldmzb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lrctoszz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tssnwseq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fxdehbsq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2awddqwyx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2shhayjqs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2paronqtv.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ivnlgcly.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zhmuqiry.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wkbsgcmn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bnqgtkjy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2utsncsdv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ttnpwale.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lpaurxzy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2jcompwms.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lmeaumtu.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pdouygur.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2otbsfjtd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jlmrktys.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eqxisoun.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qytlmdxq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2tsmvgsee.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fhmfijux.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2yovaprga.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2raerkjho.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vohywtfp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vphiebbf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2uyjvbvpc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2kyrvgfiz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uzxoxaie.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2slgsgtxi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tdjhuimm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2jrayxpde.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2yypvjywk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrwzvuls.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2netussda.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ijgozalx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2cesaavwp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nhmueuye.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vmrfxkzk.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2sgadhdsx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zsnbdmcz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uemukers.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tulrlvqi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2avufvcnx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2plewhiaa.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2qbugmtlb.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yzgeqrjz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wptccbsy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kinlygmc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2dvmnsbdt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmfpayv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wwqmcawr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2socklyls.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2npskrmbx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2ojjctqun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrnmaryv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kivbvisq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqhtxacd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2uksbyoqc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xtaivlvk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jwpjkdnp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nvzqfznh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hswanpgt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2qwychbkl.html

);
来源：http://www.52xcode.cn/Article/details/gt2zlcivsto.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rmgukzdn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2abawnbxf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bmwqtibq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2krtaknke.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2xetpynod.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2svrgfbgb.html

);
来源：http://www.52xcode.cn/Article/details/gt2nctzvstr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xjpmnrvr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2etqxhsbl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kdmhtvic.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wvwbacfp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2grjviavk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2olrmswbj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2qagutpni.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2slytskhh.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2tetawscm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yjrdczxj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rxkdmffa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cntruslx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2opzxmnmw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xkpqchru.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2aagkzmqh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dmtvtsoj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wmontmhl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jcxekpmv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2gzfndozf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2jdpnkpfr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2pcvjiopk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fornkhyd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vvxqtfyl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mmqbjqgr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2qhjmcisl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wmdjlkxn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pvfrccyi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ogudjwxn.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2nhrfrrfg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lloadeux.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zdyxmfha.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2vrbnjfpd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kawyffdg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hedfxgvv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ahniohfu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2akehrzav.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zawxutyl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qslqdasc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2castnvhx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tkqmyvjq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vszlmkkm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2vxgqjita.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2fzgouahi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2exfwcaff.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fwmeltja.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tnyihytv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dzqlatix.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2awdzhduj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2abutsjpj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yauxerhy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zqtparip.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ropbyyax.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2idayxrwm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rmxyxcwd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kwbrxjji.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ionxfrgi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lkfcxkde.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wqperpic.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ifbouxdi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2xssuptua.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mzfgtnjt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xrzpbhir.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2tyvohobk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2dxaxjcvg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2yioisrwy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jrbkdjks.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2sirwtvoq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2drfdtkfz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2pmvbfdzo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2kmhdzfsz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2guiludux.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2vazvmzph.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ycfsnvce.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tlbelcso.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sztphhwi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2cgcniknr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2jiryfydj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mtobqtuu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2syfohkol.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jccuyrar.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qeetptjr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nbilmejk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2csecoftx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2iufbshqa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2unfapnul.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2boacmgtn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sraaxwvw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2wywfilys.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cepegmxr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2htwlccgk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2cskhgvvv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cabduzql.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zmxuyjuh.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2xhzdxtif.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2aiclbhcm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ejndltfk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ltkqmxrd.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2mgxxltql.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wxvguwuw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cxfgugyz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2czwpsizz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fthqenzb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lvfbdmbh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yapykahu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2afffnrue.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zdmzmwhn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2evtzzvop.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tigyoczf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xytbaqnf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fqokzpdg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pnusomhe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lgbhsryl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2seglwxaq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rlxalxsq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fzmshaky.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wuhygwww.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ucmuhsct.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ucdxblzm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2gvcvwvfa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjecwist.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gosrepmx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mwbfmzpz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2cfelqylo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ibxajbyu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2agmsccou.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2kkrrgwub.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mzghetwn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2tmpveekc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2smtpbpwa.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2zqwsuvss.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ooowwxnr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xogpetpb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fbzuwjmn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nyxnryip.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bilqqabn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2aecthynq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2pwngqevl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jftoolbd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kaogbsvl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dowepwyo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2pjetnyne.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nlxqouow.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rotmrvuv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ezceavxr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mptdxffm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2aqkvktcf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vijrlttm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2iwznkygx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2gafrecoi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2sbcadxvd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2uyjslujh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zllyulsj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2valzsfqx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2hnpmsvfz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mjenjblh.html


<!-- 参考信息 -->