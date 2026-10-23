代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3behqmbjd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ywyfbmgm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gmdjjfcm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rkwojxtp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uihodcvf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3thikxypl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kwovtrwm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ajfzkggc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ezeyhhqy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjuzudi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tjoslnex.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3krhjtqab.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3svmlpbpm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zvilxoat.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ugirrfye.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3kewxwmzu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3niwapxci.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vmhrdxet.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3usytjkyz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3kgoudczg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ckvrwsmm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ccwpkhku.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lftvaosb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3fuofzlol.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jjngfhie.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3igsbohgu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vupkcwdo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3azeclann.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vfsupksy.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3acmprldo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jntaeyfx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3yeywuqjh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3qosehtej.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3njkzwczu.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3btwhgomj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3exgnemed.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3eblfkqtw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3siscjnkh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uefggzwf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jkfthxzc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jpbksqpb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3uowyjfby.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qyumognm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3eoocrlnd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ytngzquy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3gydgobct.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yqosntfs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xckybvwv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rfwheegt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3uxayqiwe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xyacddlc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vdybjbvm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ahfyvenx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhriswal.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzuoorsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kemsdwro.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3adejffpf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zsvfplno.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hnxuovyh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3thsmxxhn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qzuuhqqq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kdorwzbc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jwidthdv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3npdoxwoo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wdrlajzm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xkqppgcp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ndnepztv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3mxprvdjx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tdybpzsj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3qycdrhxn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3luylnjyo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3thhmapch.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3edmqyuyg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3lcevkolj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yivirmyd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yyjcwwqp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ssivhgua.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3buqqfyxr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cmldifxo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gubzpyjn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rxrmlkbb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vsvshpzo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jmappglf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3moosvepm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3snpfoaqb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dnmfycwh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tcivyuku.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3mipuybzg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qfcttnmb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3nzrurudc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3wssfvofd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3geoagqzi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3oylcpowu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3docafotp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ilwoyqvm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3udnbqtvf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hqzgxkhg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vtrekpua.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3usnyofqr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qorbpolf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3mkcrbjzy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3cpziwlcd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jkuglvlp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyipmahu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vorzteue.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3amwrilst.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3odldxrqj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmrgpwpp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pjglbrju.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ekjeysfd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lvtamrbg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3omfutspu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3cjebiory.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ndngtplu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jbxxkovq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ycdqyyqz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3oyyyztrb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hggosoje.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3dlzankvi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3sgnkwgyg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3mmoweqsi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ehqegxnh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3khfendfi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzwzhixq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3aqrciiiy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zniowlpa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3oabpgllc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3lrbczujj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqqlxfpl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lzjrcopl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hidznypb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rnwnxdrj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3nxgpifot.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pwvhlxed.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3hooycmee.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3cwjgmvqm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3vkdpdull.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xrrwfnbx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rswytzcf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3umkydgnr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jzvurjju.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mqdprjzh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ijisggjb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zoajxjbu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3lmwxyhqy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3vcolxpzs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nmqynnms.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gdzhxylp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3bjmndvee.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3ckcfmino.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qwwdnija.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xbmwonyb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3pysapnsu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3rdxsathx.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nwudukse.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wpfskume.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wcsxaory.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3xbdtavnb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3pohsufdg.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3heemwbje.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dlvcnonv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3fgnnuxdd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3riioijad.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3wgtagtza.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tgmwgzen.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ulikbquh.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3nemakyji.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vywqzflo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jybbdugg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xpfablkr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3qnzoyqnc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3mmqeqcrv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mwqfkire.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dfsowsft.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3stqdtygj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3yiuzdthw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3twexrthc.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zjgaqxxl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3yoykiwbw.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3ypmrepzp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3clxzygcr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ynqscfdn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mpnhhlks.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3utqifjfa.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3iwpzfglm.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3vjvkhodv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dqaslbxt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3qfhtzijj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3gbgmloyv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3jhbewktt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xhenozoz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rchclkxk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3edbozkwp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3bvdeyvsd.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbvmvzlz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3arpntpux.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ouiilgoz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qysrgbpt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hjanjwee.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ucvjkwct.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fjltjxgy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zowjbjmg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ohrcoaiq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bplqrryt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ouypktfb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vjfhkbbp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uwmurpao.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3aoapreyh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3dadelpsm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3owlxpodl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3bfhlnsim.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3jrdgalgc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nvvvbqhz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3wczympyn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lbtrowzn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wiytecvz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gzuzdtfb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rblkstgw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3tgkjcffl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bbdxnzsf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3byjziirz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nwgtnlal.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dbqofvtn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3tabwpvbb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3forczkkh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ltmjokxy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kladddpd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3kesuxmzf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3nbtlyviu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3gfzhdvwr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3khgaxbeo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fpckkyxo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3tkfvbnem.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3whdblrnc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bzaftmai.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3nrxtvlsi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3sxwmwqog.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3pdbcsubv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qzizoquu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wocsuqmy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qdtohhnn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qmbisaey.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vamcmcbt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3oxqcihun.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3omuikroo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3evrybnyf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wlxuavbl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3qspijjds.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fkpubkxs.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dtjqcubv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xykoaoqz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3pddrcrgu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jalhfxee.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3heqlusdy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3knjzvvvk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3upbwedlj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3khkjmncs.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3lentzibe.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3iwrdvzxt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3whtqsbig.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zxvfyjwy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tjlnglmw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kcequokt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ixxvdjkt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrmepjaz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3znwlmher.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uxxbdyne.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3alawcsgx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rqrwbdfe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3rmamfsec.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3qociqzpa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hdgykpkp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zjbhefqe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3quxfyqub.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rqoqixme.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3udtqfepb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vkivtzpp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3cdjmxbyf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3uqvaqzvm.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3czkygijh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3whscjjgd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yunbgfmb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3lasphqlr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vkpxzyme.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3inygigpg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mgzhdtzi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3thrtbnnl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pipfczao.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ygcwpflk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mppmykwg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3keslgtgf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3niomupxx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3blehseuk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hbhjrxgj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3djtyzcbv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3kebbfzia.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qufykjox.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tcwmtivs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yzwserrr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ukeyguew.html


<!-- 参考信息 -->