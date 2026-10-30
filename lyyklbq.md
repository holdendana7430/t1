代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gywkemqet.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gqpadrory.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gqisjhbsj.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gehvcxouz.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gaintgznp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gcnfnmwsq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/ghhacynfs.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gwhqurzyh.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/ghjbxgdxa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gvzhvfihr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gawidhdfq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/glxlrjnfl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/ghvoxvxko.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/goulcaybb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/grkmyvjef.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gloyxkgdv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gmosznyor.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gluepbvos.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gzdqqddve.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gunxsqesw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gyuxqukrn.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/giskznfnd.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gmooxvpbt.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gtjgeslkc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gdqolmwxd.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/greuxrtwh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gmylrxaxa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gwrzimggk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/ggdjdnkoa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/ggeamktpu.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gtolnqccy.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gaucnqkhe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/garrimhfz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/grhskeowm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gixryoqel.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/glgujqfhp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/guqqiihtg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gpjwvlbbp.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gfqzvzgex.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gsncyegoe.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/grfcyyjru.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/ggphfitjf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gxwlopggy.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gdtubjjez.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gvlznsjby.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gdinwkkdl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/grvrqugbq.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/giukydljm.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gzfflgdgc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gknpnfuyq.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gpagiwrhw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpoqnbatc.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gerawucxz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gpgbxmxmm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gunugmtcd.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gnaxqjwxb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gnncongvk.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/geouqklbc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gshwvnmkj.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gthjblbzt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/geaqxumie.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gdzqldkve.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gpqugefrd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gzbmhmumf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gxziihdnc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gjmyrvhul.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gxrnvjddg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gwqorofyq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gbnaujvza.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/glzioouxg.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gyoknkxtt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/glyesnmjl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gwwxmdlbw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gbzskzhgb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gbpqylsol.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gbjhhpkgx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gehbujphv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gnnpxeovz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gropejzid.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/geevxgezj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gvfdwrkco.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/giqrlmigv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/grhbvpsym.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gluwpkfhl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gpaanmipv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gwftzrapg.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gjbqnboqn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gjtpugpue.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gtonhuewu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/guuoaycwc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gbgcluomo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gsvekrfed.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gppijzlms.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gxqfadlit.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gfhglxpvu.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gynlkljhl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gnxwhcpbc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gpietkxxi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gntoxdelb.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gnjolahip.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gndhycjet.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gxepztfkh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gkxhzfwdf.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gbetqaead.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gbxvlnfru.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gvbjpvgmu.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gnfrxobpj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gcxzttaez.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gcoaetasm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gqkqqyloc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gnkxwcnjn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gigrdapmu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gncozjoqy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/grbktvoqh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/ganwpfjef.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gsegezoxj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/ghvkqijfo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gwwtijibf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/grrtwyfeo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gxrmbrksh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gzzzphuwa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gcmwiuarl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/godkqxqcc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gfmrgeaqi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gooyibrxb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gnmadgfzo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdklypbhy.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/goddgegof.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gpidvcfqz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/ghnegbjei.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/ghylilgqm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gnckbaxbc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gyppvoaik.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gtskxevqo.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gkkemstyn.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gzjcrhvwe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gyjelvtyn.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/grynvgpwk.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/ghpksbzou.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/geaacuzmg.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/grrvlaruu.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/grxnimiml.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gppibktfg.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gulmxorqp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gnesykwno.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gxzcvfjsn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gtvhzmqnt.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gtuskbjfd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gcpkhnmba.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/goxhrqeon.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gexpgacuj.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gqfmgatwd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/genxlryea.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gfpfzqytl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gchheecmo.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gyznjstba.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gluunxxng.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gunvededz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gawllgzuc.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gafyjdulu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gpgfajwog.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/ghaksxoxr.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gyayefhyz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gtxxdtqkn.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gtaeuacin.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gxjrzyzna.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gnumlatxu.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gcwnopeez.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gclmteczg.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gvnbszdtw.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gisktamzd.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/ggcnzckpk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/grsoakehy.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gdesacijo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gjsdmjfbd.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gnhuuswov.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gureesrzq.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gilahyika.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gjjcxysbd.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gwckslnak.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gvqndramj.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gcrtpfpgx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gpscujxrg.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gfnrftmdh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/ghvkvmigi.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gzwpzfndl.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/ghydpvlhe.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gptojeifi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gsfiykqdp.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gbyfsteqz.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gbdebpxri.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gqtsphtkn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghglovpym.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gozygvrav.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gevposurc.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gaorbaalz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gzjcnvxhg.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gvrlpdyxa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gvldbuovx.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gixaxemtd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gapomcwxg.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gxmwtarug.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gwnhecsve.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gdodaiyuz.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gtwfrqrnz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gfaykdfod.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gbbfaphbi.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gpypcxcch.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gghxcgmtx.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gadvvtzgn.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/grzfxholv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/geofblubt.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gtmenrlrn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gghxghrza.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gghekevzl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gunlwfoqo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gzinxdneh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gqpuurucc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gbrttsxdm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gkdzpdjeq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gijzfzrda.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gzwpjarls.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/glqpllmpa.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gytmvrbtf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gbjvbyzmy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gyicajqae.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gidugccva.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gchetsqvc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/ggazdpvhb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gomcffabf.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/grctvkffy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gyeersbgu.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gjfurfpwk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gcboaajyh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gdfhdeuup.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/ggisygtko.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gzxhzydkj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/ggedjuhql.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gvuxvnqru.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gnywdlueg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gsenjyihh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gwahgamzp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gdiwqfqwz.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gsswztkal.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gpceiwhbj.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gfezvxzek.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gofyqiwqt.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/grtbfffzu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/govwrljyi.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gzsbgyngb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gxzefgznz.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gpwmbwhhf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/ghefytppd.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gaqbyuzym.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gonipgygk.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gduernbzy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gewcupfwu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gjdkmiseo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/goknguybc.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gyznadtjl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnwakghfa.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gbyhragnw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gocmuuzvq.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gygjejkzh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtapmohgm.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gwssqnxbv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/getrfnkug.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/grmwzbwli.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gnprmqxxg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gxcdgvqvj.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gzqbmnvkq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/ghmndmyhx.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/guftxztcv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gzrboehyt.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/guekfsnye.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gumxdtehx.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gxjmcecpa.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gkvnqgkwt.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gzlxnlxkr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gzefjerkx.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gaytqlted.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gschklhrq.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/givdizccu.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/ggexikrqz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/ggpytwxkp.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gyookknky.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gbmalecnn.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gjzgutxaa.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/glfxnxhjp.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gyblcgvts.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gepatplvz.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gmhkuyhuo.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gignskbwo.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gcoktgsnz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gbgcmhnli.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gncyqdytn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gjputcdyo.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gbhrrfcyj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gocrtpiju.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gslmoprtc.sHtML


<!-- 参考信息 -->