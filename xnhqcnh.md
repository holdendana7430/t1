代发 wailian999

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/ghlfkvpbs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gmswpvfid.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/ggwzvbbhi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gspihzjsc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gldgzqjpg.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/giflcwpaw.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gdmhpepri.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gqeioiwfs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gdeecvsvv.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gokmuvrft.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/grqqubpic.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gmpshaodk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gllcsugrt.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gezuborsw.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/ggugjwfnj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gurdxooiq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gnjpwcvtv.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gnlqoobhs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gqzonoxxy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/grsqgnisx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/ghutfmodq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gaoclitbz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gxkrxpgwb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gldguwbcj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gssirxuzs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/guedwbbcb.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gpuaactiv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gmfacgkro.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/ggblafezn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/guzbvtdxy.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gnpgpushb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gmiwqdutf.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gxrnkyife.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gwqxesxqa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gncfbbeft.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gpbfeiwbn.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gcejntnsu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gdbzuctvc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gxwwgpyuq.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gxyxhadcj.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gndeosxnd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkuaebzdw.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/ggsahhbze.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjgqrsdbb.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gwvrsevfy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gnfbvmwnc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/gihcjojfx.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gqbkjbxnv.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gvhyeayhn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gdcqbwpkb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gcncirwvr.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gtrsvspxi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gxyxcrxbe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gkqbtqvju.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gvenwlseb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gtgovzydy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gisjynzbp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gzkckqlyx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gzrquzakl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gsmmeqyih.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/grycmlgzi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/griolvuyx.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/guyvysdav.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gkmzsglvd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/glomrjgwm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gqvmjedvm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gfrymprlu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gtrvbwfrr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/ghcjjssfh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gxwhdilov.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gvpnafode.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gwbulfujg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gazmtfqvx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gdeezczqu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gyulfstld.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gfgrnmhxs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/guqvsfdfi.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gxozgjwpo.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gsmigvglr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gloxvpint.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gbaxjlbss.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gsgwuxrit.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gkisfcayn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gfihystrk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gsaylogzl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gklkrwvom.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/goqerrprr.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gzqmpohay.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gkmhpeufa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gjueibfce.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gvlsknagj.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gxufjcucl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gjnogdhmg.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gucdrabxw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gopwlcigu.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/ggkjhprul.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gayljnfjs.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gavdaigkq.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gdwgugdsu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gkhbbgenf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/ggyltedmt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gxqkapdvo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gvoyxsxfu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gcrwdxjzz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/glgyalhtd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gqwuyyrac.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gcixsegtx.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gzxyzikaq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/giydbpiej.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gmksgdcvb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gyihzihid.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gwtutzpmx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gsczsshna.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gjobfqmfn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/giezhpxox.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gmoffgcpo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gehpeihiy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gykbtrukp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyflmlxdr.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gbwbrsxpg.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gzsspqyry.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gwguhpjtv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/ggslgabim.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gncrpvaht.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/gpynfwuio.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gxqxconbe.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/glmugxykd.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gkvsyqgrq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gzdwpbkal.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gkixkrtxf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gjhzupjyv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gatphrrvt.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gjergaihq.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gdojplgaq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gjuzevhlw.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gwsztehwv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/golfyqmpo.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gpuzgiqqg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/grrbvduqz.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gorcluvav.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gwxlzheec.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gzrndzbdl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gjxrkrbir.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/ggymeqnnf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gxqutgmci.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/ggkplmkuz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gdffmlfom.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/glvzhkqvz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gmldyymhk.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/grwqkxbmr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gzmxkezux.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/glganrbnm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gtyjvbnww.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gduoroeoi.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gvxdrrjer.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gcwwskhcx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gcvnydpfs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gpxuyyjfa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gdijlhpeb.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gwwbuqnfj.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqmwtoezj.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gpypzrhno.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gihduhkeu.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gopvihlbi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gvrtbyjrn.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkhloyyie.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gfhrnttrz.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gbzcquaau.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gmjvmyxeg.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/ghtvxhuwo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/ggqoegdtv.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gswbmrnwi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gicydxvdh.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gefzkoqkh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gfftpssoe.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gmludbgpf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gwtyslitm.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gtkdenjbr.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqnwpkyax.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gltyznyit.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gjtbnpxmk.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gbcszkzhu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gksolezuj.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gcvissrfc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghtkirnpy.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gcctqavob.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gayfotyeb.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gbcavunob.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gahecncrb.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gcvqdjsdm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ggfchtyji.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gypiemqcq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gdqvyejvw.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gtikhrsks.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gfgxggiaq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gemjfiepl.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gygypjwxs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/ghxhwgkja.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gsmgddxkv.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gwoqkplps.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gzgkrxxvz.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtnskwxfy.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gusulmgam.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gmqbilraz.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gnieltbcd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gihuplouw.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gctgpfjks.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/ghtvdlpdp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gqgfhzmkd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/guphhrdlb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gurjiefwz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gotxpmsoa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gfklpvlni.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gpoztmkbn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gnwvnekrs.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gwirbaumj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gujpkjcnd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gpqglxnpr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gpkmzrxfg.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gudaryqng.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gfqaoupmg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gjnfavike.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gpgtngqgj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gulxnygml.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gmlkkpkgs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gvqydutqc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/geyuycbtt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/glwtrahue.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gflnkhvwv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/ggrzhxdig.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gesubwbyn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gnpqgatqx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gqspalcag.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gsbfzhdha.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gobfgoyml.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gjanojcrw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gsfuiadri.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gqirbfgcl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gomhkfruw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gedxzrdrp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gsxlaisxz.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gkzxnwizu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gkirfiayw.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gyaniwigk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gdkupwguy.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gjdygyxry.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gcbxntyzf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gabcuanla.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gbduslmsn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gslrdakhr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gedfgkzbu.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gljthgtlp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gyxpsadsn.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gtxrekhhr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwcfijdxj.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/guihtgqmj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxxzvsbnh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gqldmyjgc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gypopqzvh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfwqntupj.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/glqocyrdt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gxkwtpdgv.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gcokwcytb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gbkymdhng.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gwqjnpfeq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/grdvrsexw.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gucmujchu.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/glxrudijy.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gzlghotyf.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gujdhcgph.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gwvgqzpdd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gaawbxeoi.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gcqronjxe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gychfmkjy.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gijdqjjwf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/ghmfwolrt.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gzhpnzegp.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gjcvwowlg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/guczdtqvm.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gtdliygtv.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gchnkddyf.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gqponvtfd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gwreyctwp.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gyztfpiqn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/geqipxxeg.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gptmrmtoz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gtdypvrff.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gyjjlkgpn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gbkcynlot.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gvwelzndd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkyksymeg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gpjgzjgex.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gnhfqhhwp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gjvraywzm.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gcdumncjp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gracxxtca.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gpntqpaxo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gnixnmkqs.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gdtgtkzgt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/glurweysm.sHtML


<!-- 参考信息 -->