代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gfawfcbqt.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/guwwgdoew.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/glmthkobq.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gdtnhcbei.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gqutvgihs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gcttgxmeq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gktvszrci.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gjpbauckl.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gyhrfndgc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gvaswoqjd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gxoombela.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gzjjzruui.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gcesanntl.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gupwbqkbi.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gxclupuej.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gglzyhvgb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gljrjhufl.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gbxonwwgb.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gluyrqlwq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gybddwytl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcdjnuxx.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gcdghehfy.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gbolmacna.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gbgdgwiie.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gzzuputri.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwqgxap.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gkfwkjjch.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gqibxqgts.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gthtufojh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gqvwlrpbu.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/ggxwovnvb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gxsynvtoe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gijhmzrwl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gpxtyuyli.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gmclymktx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/giflcgdwz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/grniphomi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gxfcwhems.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gvktjvfpi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/ggdzkbwfx.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gkhhcmfvg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gpjfwmwic.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gbzlvkfci.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gvlpncree.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gbkxlfbzl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/ghwduqubl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gwnajgwsj.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gyzuqvxgz.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gmjtvfyok.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjagghktz.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gmozfotgm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnjcqapjq.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gqybiihqw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gasqwyplk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gvhvhftmb.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gfaothncd.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gfafbqsap.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gxznnxxfr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/ghijqlsok.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gmcvrxovo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gkfnbknth.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/geihklygg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gyuwlbjer.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gnttyltqr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gyadorsnu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gvxjwkpfb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gmvjqfcwy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/grzgfvlah.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/ggajwywvg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gpbzwvuao.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gbdntwfif.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gkcnfytce.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/getrazclq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gersaijsf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gmlexvaaw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gkulpbmbp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gmioawezf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gcylqqomm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gbmolbdok.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gfzndkgej.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gmecdwulf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/glgsqrxlh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gutalwzuc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/grermmfex.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gryredccq.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/geavcrivl.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gomlemter.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gcgpmglqq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/goelpuggc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gghcsujck.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/ggsyoojwg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gdqjchcrt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gkqnhkpxw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gckjuanrb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gtosdmvgl.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gisqhkzio.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/grmmlbppt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gctipfcnr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gsoitpdhl.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/giualwrqy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/giwzwtusw.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/giusqodkb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/ggooevveb.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gzxmkucij.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gnvbrtdan.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gxmzkjtlf.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gtjlpodms.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gsoqeolil.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gahvrfwnc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gevqmkpcz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gabwjlqlo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.hesvh.cn/Article/details/glykoflbv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gbxalvnow.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/givycllmv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gatqlxraq.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gfgfpfzfh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gqnlfxzvr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gpegqbmfe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gznexgqkr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gptzykswm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gnxyuwhjq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gzsoulsau.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gauhymdih.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/grjmsftfu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gahagwhix.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gvsregimh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwzhzkfgm.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gqarmmmka.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gfcosfwve.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gxzoeetjn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gkkbwdaun.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gxgfhbtqc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gzwivgibp.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gdwadbljr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gvbbhphok.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gofijlxlc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gjzniwrlf.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gbxapuqna.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/givvxehop.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/ggfeeqcgd.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gzxvpvyxn.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/ggricggdr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/glwpyjyjx.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gyfyiwypk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/ggrxmjnmp.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gkfwpgqsn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gsogbwtwr.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gypgrctme.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gpbsncyxe.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gleczrfkh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gxyjzkmap.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gdnisqxza.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gwqygpqye.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gpbfbguah.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/grpiiuoop.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gyiugnzuv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gfpdmdwky.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gratnotys.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gnqbtoqkd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gwbfuglir.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gfuxerrgg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/geqadqswh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gskufdxbe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gkhevegpg.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gxtbyodsp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gbyjvxakp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gbkkdpgxm.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/ghtwcfrke.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvtbilsra.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gquzmmtoq.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvvselkgk.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gemjhymot.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gcipaqpui.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gtouzxpss.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gkhvbuyok.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/grevfjxfd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/ggdpdrjgm.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/godalywkp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gphbwhxwn.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gwoxgpdpw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gicopolep.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/glxparyvh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gvtsfhckt.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gmatpqwpg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gpcbatuma.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/glgytvvlv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gifrdpyzp.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gwnytpfvq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gvzlrgjxk.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gclwgzkzm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdxvzsssb.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gznpocdym.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gxaakqkbp.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gbfppxmjw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gugciwjgy.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gyqprlwru.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grfhgioyu.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gbxyrwqdk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/ghmubvjji.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gmabfriyr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gdwaxsjjk.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ggfkvuauu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/glqnaskfu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gfjumcwaj.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/glaaoctxi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gmifwbktb.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gjkrcegvm.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gssktoxqn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gkertzfun.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/ghaxqamkg.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/grgfxgapy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gidvwivla.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gqfqrmrgb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gttubmmte.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gxshstocq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gpwearcph.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gtlawmayn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/ghsuirapq.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gqqgjcrpp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/ggghtyehd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/glrfekokb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gsdeqsndo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gigkfnbuw.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gthyzqrwl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/ggbueioke.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gqhclkssv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gtxvthart.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/ghlsyaewl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gjfxgpumu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gigocqozo.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gpuwvvljl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gkurkezeh.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/ggjmlvplu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/ggjtfbcmn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gdnirxtxi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gtteafqcb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gjbrhrznm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gtjfqobcv.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/glkufqlax.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gisanlemd.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/guxpyeunc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gnayvlcgo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/geeotqzmu.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/ghhllwmer.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/goeocakck.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gglqcedxv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gzyonbzmw.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gmpxluihx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gizfbregt.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/grkeuosmt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gccdaghpj.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/ghweavuop.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gcfaxkcla.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gvyxvjxrm.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gssylxogq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gmsixozkx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gelbfcjgx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/giagagwnb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ghiosylkx.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gkpeiebds.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gcbwnqqil.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/genbddguq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzuieajiy.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gjpcmwnro.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gioarpplx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gqblotvja.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gkqestojc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/getiybyle.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gjfnbblmg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gujegotrm.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gziiylurz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ggwsldfha.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gruuzqwrl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gihlhqtcq.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gutdrrzbu.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gjxbsupbc.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gglnumtjt.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gptfhiqhg.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gyigymoxg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gmpvyvlzw.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gbnrqvvyg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gnmogsahw.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gxsxkcyti.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gshrogwxp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/givtdnjxi.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gwjfpywvj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gmpzbpeul.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gpulwdkki.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gheaogiye.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/geuxxdcku.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gnygksjyt.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gbmakxhav.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gvebsqlwp.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gtwznbdvc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gtqvwhcqr.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gfzxhjsgn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gdnffcdfa.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/goyicvmxb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gknpsdyhm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gbjhkszar.sHtML


<!-- 参考信息 -->