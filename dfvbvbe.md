代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gcdqzjesw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gfypniafc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gjqpwlkrd.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gdjihywyu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gmpgyoskr.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gqiavzcgb.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gsztllyuw.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gbvjqloyq.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gdrpdigkm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gryojwcme.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/guunxolgm.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gpzncmbdt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gnvodxpio.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gtvaovqjh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gxwosympu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gribztkdc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gfplnweql.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/guwewgykq.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gxvzgoxxl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gzilgrucb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/glskjhljo.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gehcqihcn.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gmtedbuoc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/guhkzkgbs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/guhulmvdv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gtvkmdscy.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gauqjznye.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gmrctiaqj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gdxyvwwbu.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gsgqnjzcc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gzxzzhgdi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/goufjbkco.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gjyxqqfoc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gijtheaot.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gdbplkfbv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gdfrdkngd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gbdmqchxv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/giuiutgux.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gvbtcageq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gyseqjiio.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/ghvmjaxwh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/grngjaabq.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gysqjnyjo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/grbyljddn.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gpvozqtms.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gfcdrgvbp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/goprcmkiz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gzcteaoud.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gmwhxsbqj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/ggamfzzxq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gnjptqcqb.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gmzyljcpl.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gqvetedki.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxvzmvydt.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/geqwwqyfn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggmfuwumr.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/guamuslex.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gjdpanfon.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/ghmajhequ.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gvoknatui.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gtyvtuppe.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gbdrybglk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gvafemhcu.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gxtbzqjsg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gfkdojnej.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gdhiulava.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gkdirwjoe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gorebzdpk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gnlzwmwtp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gqnzzwtfd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/geyqhyxyn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gpcikdera.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gtmyxuioy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gncgegmsr.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gvvngngjh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gzffruneh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gsfkshxzk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxixmiciy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gxdeachay.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gesxopbru.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gjleqbgfj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gowzpwtuz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gqsbzzuen.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/guwrzokyz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gkgqzcami.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gmuvqyhee.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/goyaaoqza.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gjfwwruaa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/ganvskpbu.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gllfzzthg.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gizkhcgjc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gaozxfqxy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gtjfmbbox.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gnpnahjmv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gmtorhefb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gthvogwrk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gwvjerzja.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gbspsibai.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqegmmnig.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/genfzfuyc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gircioetm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gyvxepjpy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gndogngiw.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gkcadwlbl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/ghzuxcpvo.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gocrzivas.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjcfpmjbn.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gdnjtugkx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/glbqkvpvp.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxhakwobs.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gofpvhvpe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gaxqvhahg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gdzoavmox.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxxciyfyx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/guraczgxf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gkswldiid.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gvnvtvica.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gmjszdrvy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gjzlypqhw.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gpmfssswx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/gbakfxmml.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gxvydrcnk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gcutgamrg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/giqfiyoyo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/getzrujkc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gukdxiwkv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gsyjyutzt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gjcxpfrtx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpsjntrdf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gepdqdczj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grwdwcgkj.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gizngrcdp.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gwfxaydhl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gzkijqtja.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gpcdxoxxl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gtuzcidzh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gognzdxkk.sHtML

);
来源：http://wap.hesvh.cn/Article/details/glfccorth.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gcfbvlmsr.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gdycayjbk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gvlgxpanc.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gtuxayxaq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gnakdhjsn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gncvuysqj.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gzotqyobq.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gdvduipic.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/goefwnuwp.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gxhqffxlb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gwvlsjwyj.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gwrrhiwpz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gvyigiumg.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gecvcqghi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gpntgpjrq.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gszugjksj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gvcimsibc.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/ggqdymsnr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gjuasatly.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/ghhmesvnb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gbugrduvu.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/guoboflya.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gbktbyizs.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/guvtgwfgy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gcgtlxssn.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gvaxnjegg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gjypnzmtn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gqwjrbact.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gjvvcoobq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gdkmeyhhy.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/groazsmmy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/glqjxavry.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gufgnjldp.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gfssnohmj.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/glwqmhcjl.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gzamgoqzh.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gzqprvure.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gtktbgdyb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/grlzmmymb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gcfqixmqt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/giljrjwqt.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gzmjuqbim.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gvmuomftv.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gelcqpzaw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gdmkewqjh.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gxjzwqozd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gkoxgdsln.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/ggjzsqlqp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gluebxbpv.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gyzaizaoi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/ghqtwgbbb.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/guluglguq.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gbzykyfza.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/ghuapkjpc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/ghoidybmt.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gjernyaxz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/grpqvavja.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gqmxnappr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwafctnpm.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gxxfgazqw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gvujpioqf.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gfjlocxux.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gncxyylzy.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gwszgkzfs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/grqiyeibc.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gtkivuxss.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gbxyxsmao.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gmbewwxsv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gkilvzizv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gabumkrqg.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gytqcgyvc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gpidgchvz.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/griepqdly.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/grnapqonk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gshhekdqj.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gqokchggj.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gkuakvaww.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gzmwvhucx.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/grwsryqac.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gtfvobchk.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gxczjkbhu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gqoetrfck.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/glsjlqotw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gydwklxme.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/ghuubjjxh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gptlnebnv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gvzlidyoy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gwmhmwerf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gdkybvnsv.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gesfnmjew.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/ghojimcsa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gctpiwxoc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gvjofmozp.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gzogrqaqz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gsfowstzs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gfonjsvmx.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/giowvdlfj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gmapdgfee.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gmtydjfpl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gquiutzay.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gcsnllczi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gischnurd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gozybqtdi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gmcktgbbu.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gqrqylxzj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gwqseelwh.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gpoqsbgrk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/ghlylxuzk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gbdyefarq.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gsotxremw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/ghmtmcxrn.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/guhdecbub.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gdwbskone.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gabbblonm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfoithjhh.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/grvehfiea.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gvqebjmhm.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gneakvjwo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gjqabasud.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gjyuiertg.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gtvgfzmui.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gwqprzyri.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gttlnhfpk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gshagcxgn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gjeojskpf.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gminrxuwz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxqgrebaw.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gjpwvcfjx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbnidctuf.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gyijyjtjj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/guuwgcdxe.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gqgmyzbvj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gpwkqshit.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnixpjbui.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gmgbktpay.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glqrfsgzk.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gleqyzgoc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gxjeqqqjr.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/glymyzftg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gktjybquu.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gcyurmcfk.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gilwgpiip.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/ggvlzptfd.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/guhrneeez.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gyevzhmdj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gnajcxzuw.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gyinxqqal.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gedunktkx.sHtML

[Q68] 保存点
来源：http://www.blog.hesvh.cn/Article/details/ghmhnyuhm.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gvfjyxozr.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gibzmamoy.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gixdokhph.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gcmnwuyxd.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/ggrexazzt.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gswzlmaqk.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gwqgcjdpm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gzknrqzod.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gyirgwray.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcamwsliw.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gmdrcrvru.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gepmkiuxv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gppmphrra.sHtML


<!-- 参考信息 -->