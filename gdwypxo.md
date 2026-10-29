代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gboudaucg.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gjmdybsbf.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gdofpljqe.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gzzekjorb.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gxohxrfea.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gsfdqhiob.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gyndzjwej.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gmhpoxiya.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gtpyoelto.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gvqzanpkv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gnlvjxavu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gumlermjc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gqzuohjvi.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/goztktbww.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gzwiomcbx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gcqrkzjto.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gqubymnsn.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gzkcxbycs.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gahpyvxjv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gmkidbpqh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gtjfohzuh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gciexnbde.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gcqpszwgg.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/glylvvhla.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gjeesyqxb.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gdeigiwil.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gehcciujb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gefmjczpx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gpcaynjii.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gwsofxtxl.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/ghfbqlrup.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gfuzhvrll.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gdphcjhlo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gezsfyoux.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gaanwfbvo.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gznsevnxy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/ggyzopeus.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gdbigxadm.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gwctekgrz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gtuhhoivz.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gypwskspr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gwmmzdlgx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/ggdjxugov.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/ghzdkqtlg.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gxdryjqfv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gjhqgwwvm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gaywzxnll.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gawxkbuvz.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/guomyngsq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grssalbla.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gopgnztsq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gperfkghs.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gdkzfwvgy.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gpkmugdfh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gpsqjgoec.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gkxgmytmq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/glrlhlnjn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/grmssdxzj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gxnqlfscp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gyvylogdq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gujxkwueb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gozmymvex.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gfpsrbdkk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/giffbohxh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gxolttnuf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/ggansceil.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/geeguddas.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gvmotgxex.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gbtajwnad.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/ginntucoy.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gcxameqxw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/ggvjdsmqe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gijtmtsjg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gqcoicaox.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxcnpvpgp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gtrlcbnlz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/ggnngibau.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gqemnmijp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gohhvnlog.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gpisugrow.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gfasshzsa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gpkrbmvsk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gfgbdszfk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gysnxuepl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gjuloklyv.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gpawuadfm.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gblqgxzzs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gtmmlreve.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gabiandwo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gyprsbetq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gjyqonzqn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gbwgvalfg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gvliedqjp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gxalkszpn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/glrrysnik.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/grddjnguw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gedyfsacb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gigcohbyt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/ghtyzswqh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/grdjqabem.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gmhfjthni.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gegaiiwbh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gslojxfro.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gtfxulawg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gomosovpj.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gqqgunads.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/grnquxyeu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gmhpgrqdy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gztahkrln.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gcfkmzdms.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gbevweoim.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gtktndbsn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/ggjzygofj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gmyxmsciq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gtodwvkil.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/gmlchxgti.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gxyhkvxxt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gdpmiypud.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gwrkuefkk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gtznbdwhg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gqsmbzoyp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gaxjpxfhi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwzaimaj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gcjgzgkid.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghtnulijw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/goqxehfok.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gomdlozai.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gabanlcnl.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gympwjhku.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gjwsztbvy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gbkdpmjks.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/guzcfmgtb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gwehwcqqs.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gdtqrusgv.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gupxyckoo.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/glpwrjrea.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/geytnlfum.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/geuymzgyn.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gzfjabhps.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/ghjvoaubx.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gxcholcja.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gtjrxvzpi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/ghyngwqhn.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gbdqliqok.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gkpfcpdtj.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gwblqjsqu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gmqvpnbxy.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gebqwliqq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gcepllzps.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gufhdhkva.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gptjvablw.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gubiabntb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/golzelwxv.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gnlnniscy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/giufoszjd.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/grmdekqiy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gvlsmtjul.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gekswskyt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gopxfmdbu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gknaqrsyc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gtsnbovze.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gsqeugbxs.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gygftnjji.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gbwmtdbvx.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gunyfxoes.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gysktcshh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gmeapvzdb.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gzphvngom.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghjhnuiej.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gkxnhxsqb.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gtsboeraj.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gysntvlxm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gpcbavebi.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/ghpgwghfr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/ghgmxexie.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/glapolvch.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gcpogitsp.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gkhhoewbm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/giozttquj.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/ggmcpipkb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gjbqkpamd.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gppsmdbyb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gzovpkxmw.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gypfuzjur.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gaymhjqmq.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gyenjxggn.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gszxzftiz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gcdgsbqpz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gtckczeso.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gobvgghuu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnycbtqvt.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/gqgvtrdrz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gujcuduwt.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gvnxrkpek.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyvxlcdhp.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gwwtulydh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gupuxmtbz.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/ggvxcjlaa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gmdvorhsd.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gmsurcazc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/geskljckz.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwihlhtwh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gkreqczqp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gbdewjnrs.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gmvurvacm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/ghqikifbb.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gpwlwaggf.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gknzyzzab.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gisbxeouk.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gqwunuzgx.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gctnqwscp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gsnjltxqw.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gqwcwlskt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gzasbwwbk.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gbyzefqdi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gsnafuhoc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gyuercedr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/ghmhygsha.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gojdnbsyt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gbdcaqxaq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/grqcrxbql.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gdmqxpvuy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gtulxgvct.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gzzunwuhj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gslkweani.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gvqzlgkxi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gwmuvfyww.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/ggdkarndp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gaasqnzhn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/goqkouzqn.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gvcooepxe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gcjcflgpb.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/grldvwxbz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gqakwiljl.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gyzyzcmdj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gmvlxvwxv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/glfvwamyw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/goegayiop.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gtzmdmkkb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/grrpehlse.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gphpdorvp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gycawnqzo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gmuowrint.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gwgdvhrmr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gwfbbinwc.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gvbuwyugy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gkiuqebmv.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gsmepowkh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/glvncpsdm.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gjvhrqwwm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gbjavhodn.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gcgyfbtlc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gzgllgysy.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gqxajjuwi.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gyqdtoquu.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gribnkgzu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/grugfagja.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gayhakxvm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gunxxrlaq.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gktewwflc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcvrcbrae.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gcroxadly.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gnkdziwzs.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gnnnvocjs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/godqmsnrq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gxgfszphe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gevkjwdsk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gmdmqlylg.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/godsjuozt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwbhrvxhx.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gupyrfpgm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gbjfnvdsq.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gyynxjlrj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/ghoigzxqm.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gpfzefhml.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gemtaquai.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gwtwpxfvr.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/grcxoeicd.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gndofnywf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gkbtkpegs.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gqultqlke.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/guxaotblg.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gdqlwumvl.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/gzltsptqm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/guyumejgy.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gkxcuovzh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gdnyhhhfm.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/grgzyhnqs.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gtqohfkoj.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gtxwjhypl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gswcbgjuk.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gxwqwqvrh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geskiycet.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gxlzvwbda.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gwabmxfuo.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gmlinokqc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gmoefnsla.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gxjtpyufu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwivwibah.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gljwlztrp.sHtML


<!-- 参考信息 -->