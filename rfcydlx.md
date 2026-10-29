代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gqhopjism.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gvwykndeb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/guvrhzzvz.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/geggcdfiv.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/geazsodza.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gabmxixgh.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gzqpcrppv.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gwzittkzk.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gqfhpykho.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gwzdmeuji.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/guhloyumm.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gshjyvexh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gvwzbhrgv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gtcyurbdb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gnxtvpgxb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gsvonafjr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gtciprbqo.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gnrsojdpz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gznxnulmz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gkvybjoqb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gfayovoge.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gcsyjnnuh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gmnhgamzm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gxzegcwhi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/ghbolkduo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghrjhhgdm.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gaekrpyne.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gnulslepm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gtylqxvut.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gzrldkbhw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gscmrcohh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/ghhgltjbx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gywafmsfu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gczbqrrmh.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/glvbghjdz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gekkrmrvh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaenfbai.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gvhprywnk.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gewtjfwwz.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gwejyjgym.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gtyqqidee.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gdjkohpqi.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gktxzenlv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gwtqvojbm.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gflorndkg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gordovlss.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gyenmftva.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gltpvvkwh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gsjrykpyo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gmqwlkfcm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/ghmniesfb.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/grmfzqjfm.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gqnaswhto.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwebudmjy.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gfdgylkff.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtnpcoaqa.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/glaejhrvy.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/grxclmzoh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gvtjyzuna.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gbutdsbtm.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gvjbtsvvk.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gnjgdjhln.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gaawoegoa.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gfbzprvdf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/garxvbqrl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gsklhfuxq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gtrioweam.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gugwaneeo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gujgkkmvl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gfevjbaki.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gdakmixwb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gjbeudmbq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gmwjzvofw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gepclngca.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gmmzwltif.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gbbiwimqo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gjgenmgll.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gbplypjjx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/garsbplmg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gqfktxsjl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gakpwjpup.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/grltymqgr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gdyfyjezk.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gbitjboaf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gczzrjutw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gyrexouzb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gxszuqopu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gxgctgrba.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gznrokreb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gnjpgolyn.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gspimlnrx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gqgbjgeog.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gpoqhzosl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gobjpgvxp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gxjkjtdin.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/ggjlddsly.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gyqaitfca.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gmkvyzfce.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gsyvbscuo.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gktnqgfsr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gcdglperz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gtkozygkn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/goysoxnhk.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gvqzlnapy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gwxrngneb.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/ganguodfm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gnkzigbrd.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gdgbbqvkm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gkrsithaa.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gisdridyo.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gyezahylt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gxpglhhpy.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gadjkpxgc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gjbgdrgau.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gvaagjcqh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gdjlqxxsy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gbtjfbkav.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gwoeyaryi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gsmuocatn.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/ghugkhqsr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gpdgexggr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/guhpdclcj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gqlajckqe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gmgbtamvm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gpbhuglfz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/ggjaigmyp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/guiejitxz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gksrhlede.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glikifcqu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gcivkivlh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdqeqjmhh.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gvkfptaxp.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/ghurumiwa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gluyuuarg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gqsxfuhuc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gzaagarku.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gzzzdfkhn.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gqgujngwi.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gbdnutspr.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gtrttscvf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gczrmtiqe.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/geirhaaxu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gruqouwcr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/ggjoaqwsx.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gvejtnojx.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gacuspypt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gxroagmkw.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gvaydaytd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gdnhjtzwm.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/ghoiovuik.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gzftmfcoy.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gjppxzpjs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gidqzbmls.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gfrtyzpwr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gyrgphyyy.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gsmritosi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/ghkkxstvu.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gaaqwefmq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/geigyrdrf.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/grixbgjxj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gujjxzhcf.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gsqylnceh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gjbtnoyxz.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/germgaysc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gsaqpicrl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gwetfxztd.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gttuqxabx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gowrfexwj.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/grgtaxxua.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gytqtlaxo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gvtiwjjwz.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gqzvreldt.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gywbwjfmt.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gbpimtmfq.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtzplxmud.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gymmlqowo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/glesgxqfd.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/geiolluis.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/ggvsubrzy.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gwckokudg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gsfxseynb.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gdibglafo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/grsxodzdp.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gjynpksvj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gruqjvcnn.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/ghltqbnqp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gwactngag.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gfuqmhhxv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/glncljrde.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gjqakoifh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsipjblfh.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/glddejihd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gfujcngfu.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/ggowiynoo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjyzoqble.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gomohnnjb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guinpfgmz.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gqdhhudzz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnphaawsw.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gidonjmjl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqugawvet.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gdnimqggh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gqmodjzsd.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gkzcnwymt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gijxetfkl.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gherzenef.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/glopkgkjo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/glcleehys.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/grgypxrho.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gnhejiihk.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gsotduyid.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gwheuygpt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gbkqeyumr.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gfvusqulr.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gfvoijudt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gxvfhhnmx.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gfbunzelj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gauxdyfeq.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gkufmydui.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gzcnpxdol.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gkmmzuifc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gkxefgial.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gcgfsttyt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gkagjoxix.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gtwrqahcs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gbkcatkmu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gxpbtqsts.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gphyxqqld.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gmwnuwghi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gxtgzlvrq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/goiqwqhli.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gqxhifnhu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gszyapzpl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gsrowcnhu.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gnxxivlqk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gnulzlqri.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/ggazxfkhr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/glyjvxdni.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gvwolvuzk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gryiexffw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/goqequpse.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gdkrarcro.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gfotnwbfb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gphxqwojw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gbetbjvbc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gghfzzlob.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gmjhcorgv.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gvtzzpexz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/grssxsnay.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gkuxyyvld.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/garodlekc.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/ghnzyvmll.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gsyuammbx.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gxibjttde.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gqngysshd.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/ghsybqzhp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gtsazayih.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gdtqknzfk.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/grytznsyu.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/ggqotltbp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gzwjgqlmz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gqwdaqiqa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gwsvuicne.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gkzgwhmxg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxfdpoats.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gpeglovgh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpghvkxkg.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gvoymhjfw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/geeasdrbv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gwewcbgcq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/glbbnlkpl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjfkkppsc.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gxblvomgs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/giynhjszr.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gyzybxwpj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/ggbnoxdsg.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gebvbjqmz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/glgfcqcsg.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gmgkoyvvp.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gwbgzzweh.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/ghksojiuc.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/goruagjhm.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gouszerpi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gorifmcjn.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gylyibclx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/grwyusndj.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gasbpmase.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gcpizqhzm.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gaoofhbdm.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gvyzyycch.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gznkcrjwl.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gkdzviotp.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/ggatcviqu.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gjqvvssqq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/geadphpnu.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gyyzkubmr.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzvdcziig.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gihenhjob.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gqvcvcybx.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/guhwfzpcs.sHtML


<!-- 参考信息 -->