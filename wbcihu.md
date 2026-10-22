代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2suhmzpxv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2lnexyycx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lwyjoceo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wqglshih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkmkcefj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2uwcftsss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2husziuas.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2glasulmg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2otyiizev.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2baqfretl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2whahswvo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ceasbbth.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nygmcjwk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wlikosse.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxsatwl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2gftelwzz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mmyomanq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2skbwgtmx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xiyffltm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2seruifpx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xzrbqvkg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lgefyklz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pdwawxhg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mwoywkea.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2peqhjdva.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2apzmbmhc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2voryvwhh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2tgcvsuvd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2brmzriqq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uywfvwto.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qukrdndb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wodbhbwr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qydgktmp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmdoyein.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tjffnlil.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2nndhixlt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xmmyuuzy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2urhighaw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mypvsgyh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vdpimhbc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qfrxdqap.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ptvguypz.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2iqlcvrvn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kvdjilgo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rxpepiux.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2amokldvl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hlzberoj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lyjrbfnf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xmzdqwxe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2lahzxedz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vhvvozpn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2stbimyhh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2cbrhrbkh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2etugwvgu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xatlqhek.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mcghggmi.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qkeymjxu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kvmhzcqz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2yjfmpcwy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fjkiqtcy.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qdfriazs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fruffepj.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jyafuvlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thsohuof.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2kqehkewp.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qzgmgvth.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rtgqvurp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gsfixazg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ckwwpirs.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2bkcljrnr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hundoiaj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qxmbmuwm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qdvvnxum.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2tcmksnsq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jyinahfc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tcvebbrd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2csqecnrh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2qkhptoub.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ickxqbjr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2bsfobtfx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bskqbxth.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lroyjpgw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fsrmybkm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vixzpvee.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tkjsjeyo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jvjzwale.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gspwblgt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yhmlnwee.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wfabzgag.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkgbtfu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2buurqwek.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ypkqnhvq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2gdbdaefc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rlmjmdvm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ibfvkfhk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mlvmqkny.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2robdxrez.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2dnovglph.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zqkbvmmn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jvxkpibj.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2poldtarq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2oubcydds.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bnuyurna.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2giuuqlsh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sktbkgrz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2teifgauo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jojwdpzg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jbsgzowx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vraapxbz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hommrodd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2updzgfic.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ogbwvawn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qbkvruap.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2idcsvqzw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mabaivof.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbwtvrdy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lefmegkg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbhrptpk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2mszqlglu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2azfgkkgj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pynezspc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tubovevg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2whfnydhc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vkrzfcvc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ehlyoihj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nzxkosgw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qxeazfrr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2ylpfuhkn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2fhtoxlop.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zazbtyeg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2raibonch.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kyquqhwv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ymywiavr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2kzvhydut.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vifmxwen.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dpwjbqsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyypslgh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2zesmhsrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcesotwr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2pogkstuw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2kpkpwvir.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hwbpeugg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jgdvnszf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jrtsngyk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2bqurbbtd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iiacdqfn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ytrilrtb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2rxcdkyud.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ynugtops.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2oyxqwrqh.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2glohqpng.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wwaqkcbc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2czmzwbxj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2knumpbhr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zfmddkwn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2agujjujo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2xoqkpfei.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jejoazrx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2wasbenzb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2rcgloeyd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rgjljcvk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xmnnwprl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ppxpeedh.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ofxrssyh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aheodqfz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ztuzzdur.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2mkdroygt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zvhvgxao.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hhugpagz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2xghmuxku.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dmkvwgqb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nkzkjrvz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hparzbqe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2gtwanzmo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rhnvdcyt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2svoindzt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2atjbajmf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ctoqecii.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2qhhtbosy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2sbevzhlp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nqbvkmpm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dwwilfos.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tfvxvphu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vdfwcqwr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2dnhofvtu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jxwwlxgk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2sosmsjox.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2issdlseh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2boxwsoxr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bivvnlfl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rfjrgvtj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2kocfivek.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kacgyasx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hqxelsnk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rfybckbd.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2hgfrwsnj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2sqwluqba.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ktpbgowf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmyoyzge.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2qzxwzcek.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kzkavrre.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2shqfobig.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dwvypwsf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wunzzpdc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qyahxtpa.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fddmqyjm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ubuurkxe.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yfkwdkzj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fnethxjl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2jepzfdvr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dukyevfc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vysjyred.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yjxfyrac.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yalmbezf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iiefixwk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ujdwvuwb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2vhnaijne.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2eyofwvel.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2cyejqkgp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bswbpzup.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bpewicrf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wdttnwpa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wdtfxufv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lvtvohfg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2iernufty.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2snqbmlqj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2sfshztgp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rajvswey.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ocvxdomt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2szmnckfl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2cixabteu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2gdffkveg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xccpigma.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vsfrdzgu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2deewybtn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2nthuzgpb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2defxgjml.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mmxdazhh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2gjuxnfdy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bcgrzjbx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ofdpowuu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jlrgdcei.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sfwoqoeq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bnijwfta.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xpmzzzho.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2gmptftko.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2gebpslng.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qqnddydw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gtvubhyl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xmwaymal.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kzssontd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vipmudvy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xhfetslz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jzwqhfuk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wyleaobg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2cozbdqxo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ohqcvjmq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2muviswzu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xdmgmsbh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zxibxqwt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gnppjfuh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2gpxmnxdp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2timrrecu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2chqmkxts.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wglgasaw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zcphkkzx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ovcbouwm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gxcbveeb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cfmrdnpg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lxivghxu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2yskcgfzh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2rspqftgn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2okxtyfav.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fohbpvuy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hsgpojce.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wusiumum.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aaamhlnj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lqwtnxtx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2psmdcnvy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qiqjilys.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qgzbhzkq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bjphltpz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2meufesdf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qxncxftx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2cectxvja.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2cvqkgxez.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yfymqhtf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mbacagjf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2yukatwwb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vxxmtyld.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rhwrirhe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2khfuhjke.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tyerqdck.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xdfxespa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qccjfgde.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tfveupiv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yfmjlsdd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2hwyctlwa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2oaynswhp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xkgbqgvn.html


<!-- 参考信息 -->