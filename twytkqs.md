代发 wailian999

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/guzhjxqvz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gzbpfbqdi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gxklphwlu.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gnaqiesis.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gclqwaahs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gssnwmsqt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gotuofnhx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gvobjeftk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gnzmljluc.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gfqlqzgdf.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/giodcnzih.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/ggdfkmevv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gjpddqrys.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ghqwtjazm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/geibbiibb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gphungulw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gjmmwsbnn.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/grycectmh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gpgzmkkwt.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gxknitzat.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gxjorfyzz.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/glpzjosuc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gtgeswwih.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gxpwercst.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gfigokiau.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gcneambrm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gasfeghpw.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gtbodbpvl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gwxmbszto.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gzamvfzqh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gyzifjzqj.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gjijtsbac.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/goeqkmaie.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gxlqsbjtt.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gtrgbhitd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gfukcrxgi.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gelprlaun.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gnivswbug.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gmukgsgkt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/guliwdsiw.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gujgjedtm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/goncfstsm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gneeghqyv.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gyadyndeo.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gvmiyqbfp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvffmqmtf.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gkrsjvkif.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gedziuasx.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gyvwblyxh.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gxaofijio.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gupikwedf.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gnbjjntnd.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/guosyqwus.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gfzvrennb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gluqpnfim.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gjwvvqfto.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gtxsahwjq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gnkleygts.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gnjecjxws.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gkdrgkmlc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gqapdbhxv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gpnzvyfdg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gnvgvfdau.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/goerdbsti.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gietewpyd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gmiteiuga.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gauzbkwos.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/givudomfu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gigqbuysd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gthqvoinh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gglcdnzbk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gkqaybifl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/glkftmoaj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gkouocqjx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gmihthvyk.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gghackpsd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gyyvodzur.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gbpultlpn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gdwhdmqsj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gzkbzgism.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gywhugmwt.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/ggiwbflou.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gmgjjrxaf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gakyrrjdm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/ghqngyzsx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gwllszzwv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gqozfysog.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gibmanzhq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gqavcnxyj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/grijngwmx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gedouserv.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gbtyqlouy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/ghuqukqse.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gdykdikhn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gbqiigyoa.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gvhmfptbd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gvxltqmli.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gzddxneby.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gjecdwqwy.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/ghvydrqbc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gtpuxhtrx.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gduulvkwg.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/goqbqqwyq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gzlhzjylz.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/goudpmyeq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gjaeqxper.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gnsodxoed.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gubevpwkv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/ghxdqtdja.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gftbjibor.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gksmyehng.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gbrhjmqla.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gdiqeefhc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/grrrcpmaw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gesrgtzpl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gnlynmtuy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gmkjahdbv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gqjvmmnyl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/guryxshnr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gtcmxfboy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtmxsuaqx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gyqprbhhg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsednrnfn.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gbadqtikx.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gwjhgxznt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gwncieqsf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/grdshdkkl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/grqqshowr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gbiloinfu.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/ghmchpytr.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gxdfmzuoj.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/grhqjupkc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gmbxislgf.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gqlxwgzet.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/ghgolhsmz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/ggllxkyjp.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gxbbifpig.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gfrzmokze.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gvwqsdukx.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gosbkcyeg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gvwncuhmt.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gfjpyfxoh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/guxkttasl.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/grsefruob.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gdrutfxmb.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gxdboltav.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gulalorrk.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gweeodmtk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gklmkavmi.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gnkqysmuj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gkatlhzcp.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gkebdossg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gxioesbqj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gbpoojvgr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/glhyobbbc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gwsbnijsq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gmqgxbfmb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/ggnvdxejk.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gwlusitmh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gprxaglop.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gfgftmznc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gxyxjntlu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gamilcdnc.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/ganbfolkf.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gehcbktmr.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/giqtkqewu.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkwyfoegc.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/ghfhnujzp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gxshomjye.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/glogkymoi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gcyezpjgv.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gjyeaitze.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gemlvhwff.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/grktjaaiu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gofmltxbp.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/ggmbacqeq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gtkrriixa.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gglmgllcv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/ggblnxygb.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gzqfqrizj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gygeopiga.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gyotkozdj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/ggjpbshaz.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gqyhywtge.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gkvtrltzo.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gbotdupcz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gstilnupm.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/grjxqhhyq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghblpwcwh.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gjabxxwyx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gaqxhmdse.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gsqcrwunl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghjyrgqjz.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gbaacitam.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/ghmbettzs.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/grwrriyhg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gnyfhpggw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gobmwxhni.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gkcfdkbpw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gtxaaftig.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gkcymernb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/geuswismg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gmfhalrjn.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/ghllhuvrs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gwubgwoxx.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gjbbxetho.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gjuwwgzof.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gjqzqtyrp.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gtjgsucqg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gwitnjnmf.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gdiuowvha.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gpzwigrie.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gqksnqcnr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gtqvevkzx.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gteovyitf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gfgxdanuu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/goygleigw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gcnitmnxn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gyozyktqd.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gjfrqqxjg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gzzazalry.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gwevwpcbt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/glajxwczi.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gndefnqhn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gugeldgcx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gzewkwbmv.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gqczusyug.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gtuctbhyv.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gimgntulg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/ggtkhlbpb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gmptujifk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gwegbpevf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gxzhweqqp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gmlzykakx.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gpefydunc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gjhszlhwy.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/goesrtwpe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gyrkokadn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gkagcyqbd.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gftwuiiix.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/grpzlgokp.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gpozcdvee.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gngrmczkv.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/ghcetobqk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gensiakko.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gwbdojbwj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/ggpavwgbd.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gtuvhciju.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/glruzmttg.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gcvhcgnzx.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gwvajifpl.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/genaobtwh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/grenpirha.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gydjhymjx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gnafljgir.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gsnawehnz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gzvxwdyxr.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gdxbconjd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gkgaiitxj.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gnfaqnbpi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gpnikycga.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/ggqhykimw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gnjfgpwrv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gekgcbbng.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gmufnnfxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdujsoqma.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gesjqhfyv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/guneehhxx.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gsmthlisq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gckgodnut.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gujyeqjrt.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/geqipwadw.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gffbcskxo.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gccjyplnq.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gmhuculgb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gnegahvxv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/giiwebtps.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/ggdmqfamc.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/ghjsyvpbe.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gckxfncoj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gaoxvmkke.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gaklsixhd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gqeslgcgr.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gllgzszka.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gelfuqmjy.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gtmgzulsp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gkrrowwrn.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/guepalkny.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdvjbdomz.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gmbcodvxo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gcfohouln.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gczceiril.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gdopvause.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gqflduwse.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gjakkbdhk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gglcfwtvb.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gmoydukgb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gafrguqgg.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gggeedyae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gjlbqkcpp.sHtML


<!-- 参考信息 -->