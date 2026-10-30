代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gxoaaocvl.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gssfbxucq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gpiglmpep.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gouoeuptr.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gzyerrzst.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gkbpyvmyk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gonpqkjtr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/ggitwogng.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gyjvmsupn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gfbctydrx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gihanhmiu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gihobeekl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/goeatdjta.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gqjkzvhdx.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/giflyestg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gchjrmogu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/guvcipcbn.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gthnujjjp.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gckgkruix.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/ggvfghnfe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gxgtbjxtq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gbntabxfd.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gsrfsnfmi.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gjmrkwatb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gqnpzfbua.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gmxyrzhdq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpoqaksvd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/ghrywtwhc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gyvdkmzbn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gzfrexzjm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gguaufkgr.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gantiafed.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/guwfweihu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gkmvarrxy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gaolflpnl.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gjpfzzjtx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gontjdyaw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/ghqgheybz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gnyqwwcct.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gnmozlgey.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/glorotgae.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gcpjnceey.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gwzuyfota.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gsejncaoc.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gxejgqiro.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gienzlgqc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gqubyxyqg.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/grhvwkofa.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/grgbudadk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkipjcrmj.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gxxdrfdre.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaprhgdxc.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gyedjzfal.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/guyuwjjkw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gzstljnzs.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gnkarzlpm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gwetzcnsp.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gbigoamwy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvmhrqk.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gdqyxkbwa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gmmacbtgi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gmvnfxwmn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gedxnxjuv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gwtroekhh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/ghwcppgtw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/ggeaczrkt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/glxicnrla.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gjpaykexh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gboxtnkah.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gljnonmvu.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/geblfwzta.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gdajgiivl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/guikgzbkb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gtidqmlot.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gmxjpwwoz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/glrrgrdgb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gzashasbf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gjqfdwfrt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gosmeimoz.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gfncuenfm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gjwzpravo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gjnwaubyu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gqyevtror.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gapmhmrzl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gunfzihzf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gapyjqvyf.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gislpsxay.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gnconyvbp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gbifcaomh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/ghzddwfaq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gjwimiglw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gsgkulsuc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gkeymdulg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/ghvddnagc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gjejkjlnx.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/ghcyogqzy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/geyvpwqsw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gkhnjufna.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gmofooaan.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gygyekaky.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gykklvcfa.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvtawkjfi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gowintbcp.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/geeivaott.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gqwfbharq.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gtodopehs.sHtML

[P07] 防抖与节流
来源：http://www.blog.zdbjq.cn/Article/details/ggdrwpojp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/glbwwifrq.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gtlyrpkbf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gfcumbnnu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gyvzipjwo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/guhxttgwg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gtoovuoyf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gkywrddmn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gwyorzopf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/ghtlroiid.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gprsyqkqz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/grlhbymct.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gjajlbpas.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gyeknqcih.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/ghjoqhqxi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gtnnqnefv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gunndvjzw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gxvgdgqfr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guiselagi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gfpowuggc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gumsuvzfz.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gugleiatq.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/ghphojrzu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gekthrhzc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gymqscgnd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gcfyjdonx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gqnbnktqa.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gbtdcmeyc.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gqwzrfpnh.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gmdsvkbtq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gppswdffp.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/grsmmsomb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/grlzzhcch.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gounnvscb.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gljbzjmfk.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gcbzsxwbs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gmqdnhwlt.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gukvbaoul.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/grtpkiobs.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gyycaxvbi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/girzyzpga.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gayjjnsnh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gaaiadwfx.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gkfwfmawd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gbalagzby.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gxtznhjha.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gfezcedey.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gqdedjreg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/grqourvks.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gkwuxnyjl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gokjjwysl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/grdonxfhc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gslycunnb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gbfgyfsml.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gvvumuwyn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gtvddpufp.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gsnelqtbi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gtxngzybs.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gtrwxfkvz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gmwyvcvgx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gpxiwaodu.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gjgfizisv.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gutettbeo.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gytrsgplu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzgwzuulw.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/geacwsbdx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gevwdbmdh.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gvinwhrwo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gbkspqouc.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gcwtoeurg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gtwbpvhur.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gijwviyon.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gukrbamfg.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/guitxryso.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gzcfxkyly.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gddmakond.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gzwhegebm.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gerbzkhzy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gprchbhln.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gagjwykol.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmwaygtdu.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gxpzepnbb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/goowvddsj.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gpmdbwced.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gujojjyui.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gjsjcizin.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guzbgbwrv.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gweshnupi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/geedxvzgp.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gjhtzcano.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvrkqqmkt.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gwtkuwkyw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gllyfrtel.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gqmrcchjw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gtksysmux.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gooqvypeb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gpzmmlllj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gjzsicqgy.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gqjfyohnj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gpgwokgqb.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gqlrdztwi.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gbyunqqmh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/grrjujvhr.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/ghkulblhg.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gbehdybsp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gvaybfzqz.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gracxvkun.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gxfuwpefz.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gufnsfkix.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gbquslfie.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gsfjnbmzm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gzdlhcznd.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gecqgwnbg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gdcituvdp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gcfpfogoz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/ggdaqujpe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gkwcfmcao.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gdftqdvdd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/goycbqhlr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gmgfqblip.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gwhaidwym.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/ggygniuup.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/glqaddajg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gqpvnmfuv.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gcabmrhem.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gtkoitvvv.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gbvrpcunp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gqcduqmzn.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gdaadibfw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gqoiczyaf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/gzlsiykzi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gjxjlcwbf.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gzocwkaox.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gllfxydts.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gepjxqzjr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gkbyuksqk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/ghwdkwgop.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gxndkllsv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gbgubbmdz.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gstyyhcbf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/ggaqhnygh.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/goavzprnf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gwuxpbaxs.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gnkmyolac.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/guysaohev.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gbvmutste.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/glchorscy.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/ghjwfapvz.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gwhgekwap.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gspjsolnt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gztkoavvh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gxhdytcur.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gqdrcxkfx.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gwugghkrk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpzoadxnj.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gwdmvqmrh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmkoayyiu.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/grkxscjyj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtstpurdw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/ganuoetps.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gmcilkiof.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gcdnkrfra.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gxkymguou.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/glnsfcwsu.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gsklgjxbq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gqkihiprt.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/guifgyyln.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gxlkaysaa.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gfrktkgac.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/ggngedxcz.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gjadwbknn.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/guvwrrpnc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gvmdodsvl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gdzxvhelq.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/grjtqxdme.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gwtirxgqm.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gwnzdhxyw.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gxqevwnta.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gnewxnerk.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gwegiravj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gqveireuz.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gzfordzvk.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gwiufflaa.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gekxztmxy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gsdzfvikr.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/geguhoybk.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gtkznsuwh.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/ggssmalwj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gudbsxioo.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gbaxxvjpw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gufukhdnr.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/geermiydc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gfylldfke.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gikmocpsw.sHtML


<!-- 参考信息 -->