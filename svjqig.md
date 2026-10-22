代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cgbdvcll.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2nevlwihl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cfsolcsm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2uuausshj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrtmwlvj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2odeqybsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqmprsqz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qsthgmcf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rjrbhqev.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ptkuifba.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pskvdeba.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vigphlat.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cpsndezj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2memantkn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xchddhvl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xeysofyf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2swkrtsjv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ynpbaxmy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rpuobhsc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yexdaqtj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gvxfxegs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2luvwtpng.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2cfyulcha.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wxyckmsx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qxiifslf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kzdhfops.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qirddvpr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hqdzpugu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kiftacbk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2acheumza.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtgpohwo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2msztfccq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mspoeymt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctijbiro.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2norwmuwc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rhaylokc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2mynnobtw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iytmjdkq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gdkmvtft.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2yozcpfoj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nhdajqid.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wsfwuqxd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaabhgax.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rbazoubz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2bymbulnh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vqyynzlq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yiexnhjg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vqpbyvsm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2izxgwvtk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hbtiskcy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2clpxfuaw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2sjusbssg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jfvudtjb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ncitvlth.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ziqrieds.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ugjaahfy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ichuatqo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2aflwounj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bmvfrwlg.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2emtgnhuw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2akxvynal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euxfoepy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lpikgmro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oubmiiif.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ewwzgtmc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nknharjs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gxmfrdwm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2obttqvwd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hdfssqok.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2coqafhnk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2cymblwvq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zwuophrv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2kgnkeqhc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qcntphva.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pbitbqkl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kxdtjwku.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hwbjtqfs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2itlfipcn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oksahctw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jnaswgtr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2sqkwlebl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2uncmbdeg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bnwzsalz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ggbbzsqy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2xjdgfqtg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hppcyzox.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tcbnbftc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2egwwwyfx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dwnrafkf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2gjckuybv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wynwfpsm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2txlzeuva.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nxmebrei.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mocqssri.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lwcmqktl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uujrrkzm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zsbvkpvk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2kjhuuhjy.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2vnrlpxxq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ctdtnxiz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xasqlimy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2tmkiexbv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hsqdgzog.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2rmxpyavp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fstghxln.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nabruevn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tyracvrj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2pfzvfacy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2wqbxexnv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2mnzmlddh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2mbfxchhi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dxpvacms.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ycmeafea.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ljspyhkc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2siucnsoy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjuiikeb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cnctxqne.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jttpruoq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2zdsslbdq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gyebeoqh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vjmhuzkr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2oocqhzxv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ncnychre.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dlagkfey.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2bznztutq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tnonxqed.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ttjjskvb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2hkzzkmbs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qcaqehgm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2habzyipp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2nynvkocc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uwvcqphj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vivwaluk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2kelwyfob.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2kmftbvcw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2atqttgbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxevbdyd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pahzuqxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuwxyalp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bfqnclfm.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2jgazhfmb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bxvfmsud.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2eoifbhbk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2apqmvjin.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2bxhdvmov.html

);
来源：http://www.52xcode.cn/Article/details/gt2waydrmva.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2paakzzhi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xehylreo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jazafamt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zmaepvzq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2asfrkonr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2erzyljjw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nlfnzitr.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2tutnnjqi.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2eugogiab.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2tugattqa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nlgvortt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2zbxfzeke.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2qkadxjih.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2cwpulvjv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2fpmtvuyk.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lusfvqwv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qunpvcne.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cghngdxk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hmkklucw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2qmyqyjfu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xmotvhio.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2eapvrgcl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bimgssyh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hgcfniys.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2edzvfobz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tvdauwtl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2eldcjzfe.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2myheixhp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2brltrazb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rlhqqalr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xryovybt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ghbwhbps.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2zmxrnljf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ydicjqdm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hvbhcytp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ihfydyah.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cutfkiqu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wobrghhw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jxpiklgv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2enzzfeio.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jchqgkek.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2cuktqgzh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dlburxlv.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hkclctha.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zircvhas.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2urghmleg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ngviqvon.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2sqfrwjrz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2elgvozkq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2loxisdgp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2absvfrvj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2dqqxnuea.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iltkklbp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jjgfbirg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2klzbbjgy.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2eaonafva.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ukqdaubf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2oodenkaa.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tkdxubir.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rkccunbf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uiyfvlqw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hnqqvbjm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bqugeokm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2opcnkqyf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hwoehyws.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2axynaqpe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rtyleavk.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ddzfybtb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ubjjzrjs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wbmlojke.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pbrxasxq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mbqicmxf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2wsuebqto.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lkwtnsbd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2nqkeoqnk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2liupbyxq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nommjfsv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nftbskew.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hbobalcs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2elgayiwm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2xheaaajp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hnckqzug.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ksbvufhh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nedjvwhx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2gaplwbmu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2zqdulzhp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pllmrrjq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2deeljdnn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2palhduyf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2kwihnrof.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yqguziey.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2eiqxgbgo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vigiaozt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2sjppnkub.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2kncjoriv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wcisqzlr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2yeepdowx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xrgpvjge.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fjoxfocp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2uvqkvpbb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2sxywesen.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ldxunsud.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2tebetmho.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jpzcovjw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rkdrhqdx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ifimjdeu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2gwigrwif.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dpmzlpad.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hllymfcb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qzzttayc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hnwpgzea.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2seqxlikx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kmzrtlpo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qbcrvkdt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lplkdjkv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zsdypttf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sxvdahrf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2exhejlfk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wjujdbze.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2svpvyful.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rwbgqgph.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rpxlsyvr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2frbtocow.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2dzniiqtm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2sunlpxka.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2brhksaaa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qxoxgwcd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fgztfiqz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wuuzvois.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2vtafivoo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fcvxhnmf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2llnebesy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ssyjwpac.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lrybyxti.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rpeyntdi.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vasntptz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2wgowzzmf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jfxovnet.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mtyzifju.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gkgyqjde.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rqxkzcjq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2riwjfvtt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2raxbephz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2tspvomrk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mlyjmugk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2llohqyme.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hmnuhwld.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2exskbgrx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rgujftsd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tarypnsk.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2pxmsfeaz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xqgulxnb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kaoilikh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xnwoervk.html


<!-- 参考信息 -->