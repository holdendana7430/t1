代发 wailian999

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/guekmsimc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/giwoxeyjs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gpqinnasa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/goktrnvzg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gmpbgslpe.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/ghkbwmwrl.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/glsovzlov.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gpvnzqxyt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gevnezdqf.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gfjircqsj.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gkkxoyzdq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gayauglol.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gpjbbpcyb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gbztxsyxq.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gkqahdakr.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gxeyqrlui.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/giolcurgt.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gacvjajcw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbhgyiwcu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gxgukywdw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gapvkkuyp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gbsvgxbdc.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gfqaznkty.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gocuflwcz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gbelywvoo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gcoeqrycj.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gwjjybnnw.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ggytdmmfn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/ggmvuxell.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gbaxpnmpa.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/ggksnolhq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gnkfjzehx.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gatpbudyz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gdnjffoeg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gtqrgeaap.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/guhcnwcru.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gvavzfmig.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/ggmlpfevs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/goznjsryf.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gqewtfirj.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gkputaafm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gywbuqhnj.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/ggwtzdspq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmvrboxnl.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gznuyprfu.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gvamrtjmy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gahcfblrv.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gelbokdsa.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gqnsksklf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/ghwggqmwj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gpzafskaz.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gbahiscls.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/ggqeefynr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gqydvzeoj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gnbsyxvoz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/geyrytcar.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gahmfgcgo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gbhkhkvpi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gkdcuoqkj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gyapfpkxn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/ghzlvsynr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gfwjadbzo.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gzohaoudx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/guaxeilhv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/grcbxyplj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gxgwzqgul.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gybmzbway.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gfcmtxlzp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gczlhsicx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gqhtvrrwk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gpshalnmn.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/ghtfqaaui.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gblgorkey.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gxgykmtax.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gixqczkem.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/ggudrjlai.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gedfjrrni.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/ghpqnhlco.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/ghrmibztu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gjvmaqunh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gzlmpozee.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gjrzmqibt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gkgihqkxj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gdnoruiha.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gnwhpydif.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gbohamfvg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhrkkwzx.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gugysstaz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gcfqojvja.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gfzcoyvcq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gwdjllcnk.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gaxtjxeun.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/grsfuhirr.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gbbsnumpf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gqxpieuor.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gwlwflywo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gfqwczegw.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gcxekgyuo.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gxasmylsd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gaemfeten.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gxbigqhqs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gjctjrcmx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/grukxrfnu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsjpqiumq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gtfashsqx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gjzzwjqwt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/golcmoxnt.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/giynegqyb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gifcvjves.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/grijvlhmx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gcwvcyokm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gmxikjmno.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/guxgijnmz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/getgmugvv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gmtwlevnm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gxeszzbfe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdtspgttb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gggznxexr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gufghwixf.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/glrsksjuf.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/ggxyskwrk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/guecrhrpt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/ghzoervyq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gdzfitrta.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gdcepjxfp.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gddlwqncn.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/ggrulddxp.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/grtrwuppz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gsteacipw.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/glnigqozy.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/ggujevhgi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gmowgwofn.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gzwacmsqm.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ghlqfshbz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gvyxicnpk.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gaylxuggx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gnyoeprjv.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gskfllbhr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gozwsgduj.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gdgmsylfr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gpxlniofc.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gwpmynzze.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/glycfpbtr.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gvavhepfy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gzuizfbmm.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gehdyievg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gjnaundgo.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gtnkqgdgv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/glwbjhjto.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/ghlroczsb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gmxsdwubs.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/glcqzrxtz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gmmlutbbp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gkkgzzsrf.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gcqppfxma.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gectyaqbn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gqawfqxcc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gssnzmqxw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gmmlgyanz.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gpxquicqw.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gbpqwajdf.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/glohdcszb.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gtbrldpas.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gkxeheyqe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/girfaguby.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gcxzwsvuf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gwgfqtblq.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gcmnvwbit.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gtbpqxhqv.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gdddavxbd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gpsoptzwv.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gliktgszw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ggqpimkfe.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/girlmgmmj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gzmmznhln.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gvfclesbt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gccuegyis.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gcrldjwtw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glzuyxote.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gjlcfygst.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gbmzomzdj.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/garskmwid.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvjihohcf.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gsudmjapq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxbvvwfds.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gtchddfav.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gesezxjge.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gwukfdavn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gxyfutnfl.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gsdnswktm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/giquuersf.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gpcjtrgpc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gjbcoohor.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gevsbkhxa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gpsaefxpr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gazjwbbpg.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gejbiczbo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gmcejursi.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/goyvschjn.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gnpadtmfq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gcyxhobeo.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gabbzzkby.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gfrwlzbwi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/giwqlhdml.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gprojmlfv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gcpqwrjoc.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/goaejbfqf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gckgldeqk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gyzhwwlrn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gkjxnfvhg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gpdqfbliq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gciwcmwxt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gfyndwoen.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gbeuaivbq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/glkibesef.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gtffkbnnb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/goqkqdkkj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gveujecdg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gvqwdqmfh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gdpuwhpzt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gzjfbtddj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gpiuqcojl.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/govjuegrk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/ggipcfodb.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gnwgaywkj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gkngtkrpp.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gouqbnsvq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gbrnjlmly.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gcyceviuc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/girhkvpnm.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gkrhgkdbc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/ghjxsbzmh.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gtyixmalb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gntuaylim.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/guwxudaow.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gjztzbuoz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gnbfptjje.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gfvpwsacn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gdegqzfru.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gahqvnahz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gpsefrcep.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gueurhqid.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gxgtjwtoy.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/ghyfafzjq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gqqsngsjo.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gkdayzpln.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gciejvney.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gkweegsmg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gcbxddyun.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gegjgmhrl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gvczcqrdi.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gzvzjkxll.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzifwvsku.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/guwlilvmj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gqqrszzhc.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gdanqwehl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghdnmyvvt.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gllnwuihb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gjuskkobn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gcvzvsvab.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gysegkara.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmiifelvg.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gkvprayvh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ghoddsale.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gvoudcffm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gunwpohge.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gnzumzbzn.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gzdaurcdy.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gdwofohyh.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/ggeyhjzzr.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gqqiirted.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/ghrwpqopg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gurltleuw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gyxzpqbnj.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gjbqlsduq.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gjmlzmxam.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gczkujrod.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/ghtyjhfqf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gkbeydwdr.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gmcfpqfyd.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/ghxsivozy.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gldaslowb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/givfmzgup.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/grwisvnao.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghcwmnruj.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gotnvddki.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gfamqkyaq.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gqlbiilqo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gdslpwbwp.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gvgduqtcs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gcimxdwhr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gcodaedwc.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gbhqddhub.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gfomffekv.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/grusbhatn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/grdmgwbyj.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gpvrmxrvj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gopfgawjp.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gbmseilpn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/ggczdaejk.sHtML


<!-- 参考信息 -->