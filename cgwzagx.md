代发 wailian999

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnfrrnsey.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gifxsnymm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzelwpwhf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gcsnpxuqf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gdoawnsln.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gagtczhwa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gnfslmgqu.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gunacljig.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/giciichzy.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/geaeuwdwg.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/guuuxcwjw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gnoywfdvv.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gmkowazlz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gwasifqok.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gdgtkhpgq.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/grkkftifz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gaukefjht.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gvamiovwc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gijdyfmxy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gkwdwpeph.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gmebjluqz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gqaxoxwab.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/guuvmqvmf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gevjtoiel.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/guawzrcbw.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gnovwkiez.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/givijapbb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gvvognzck.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gssckuryh.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gmrqqjuhc.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gkgxnpzgi.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/glcenvnav.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gmssrxjse.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gwfgrplms.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gbpsrwpjv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gipkruhfd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gzvyqppyn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/godnngsmv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gzkpalabn.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gtmhbokug.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gwvpshijd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gycginkrr.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gioiepqka.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/geqmlvyjo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gfmlntyie.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gpdbzdkyq.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gdkjgelxo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/geapbbkkt.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gllyogtka.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gmghhgwax.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gyoluwpgi.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gukbupblx.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/grbuxpsof.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gwizsuxcp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gwfkqnhda.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gloyjvksf.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gaipercie.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpqgirbcb.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gkvizlphu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpanaraxn.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gggaraxsf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gvpvrwfnh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gtiouamho.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gmmfcuaoa.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gsqhbfhoa.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gczatntvj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/glqewvthc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gbwzqikal.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gkeyekrqt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/ggrwydfbf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gxjbmkryq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/ggvjzitto.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gayugbmss.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/ggzzlmeal.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gdtxjgjvv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/ghpkemxld.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/goyajxpzh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/ghqizvsyz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gzzqwjavq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gugqafyoz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gvimvvyqy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gvxhmlsmt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gzggvxufx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/ggdwvxxay.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gydocopqg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gjrdxpkwz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gcafhrmtb.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gfacxhlmi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/geerqtpdu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gauqjkmli.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gbwmbfibm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/guweajkas.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/genjcybuh.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gsleimhii.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gjyenlbkk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gfpdsukvi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gulefrcio.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gjohloogu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gcwwsfyrw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gltwbtajb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gtudscinh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gylhjeurg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpmesebl.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gntkkoodm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/guvhvbhhu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gxjlfotqo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gwzdjwdya.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gxhhupdrh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gtdukfkhm.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjhjssvif.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gvfvmdmiq.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gcbbtlscn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gusfvnqup.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gbotaqhus.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/ghumxprsv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/goezyfsvr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/guovcpmoy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gnmpufwul.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gzqaeotsm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gsrbrmfcp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gkcjwnchn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gxczzraut.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gvanvmgdu.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gkocmmudn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/grtqllykm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gtysbtglw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gppkxukmu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gjyrseyda.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gyeqhnajj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gvmdosati.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/govexwafh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gzoqxpfre.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpxlaljrf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gkwvxfuzw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwpceertl.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gvapeeipo.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gwpbnppmo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/grvtwocoq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gdmmbikyn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gyablmyqi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gstlvdxds.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gnytmikdy.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gwgddiuud.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/grmxhrumx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gaixrteqo.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gzbpwfneg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gwhoofrbq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/ghcgddeck.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gapmqvhxi.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ggutwozvy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gsnuepnnr.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gbypbuiov.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/guzednigu.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gxzzkxvjo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gbksakhzt.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gxeptlfbi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gtwsvuhhj.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gdlpngkze.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvfscridd.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/ghqbgtzyk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gezmqqilk.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gbhlwcobi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gxvpcqdsm.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gkovyyqrs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gjocldkfs.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gletjvgzw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gxpbxryhn.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gxcbcmlzf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gpwsigwrt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gihdztwwe.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gzwxfihio.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/ggqrpedpl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gpeyibfrk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gxjmgldmv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gqexckyao.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gegfhesas.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvhlspzdt.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gyrwnwlix.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/ggifjlwfc.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gqdzavhbt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gqslszoic.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gvjwtkeiq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gxuqxaxbx.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gmbqrlnff.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gnvpbztyj.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gwavbdnyw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gmduggvvy.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gmlgzxkku.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gghtsoddl.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/greywejkx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gtdindllr.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gzfrznake.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gmygmnvqq.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gaheuohbd.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/ggobbcwuk.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gtxirkkhv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gvvpihhwr.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gduularwe.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gltjxhbui.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gacrzctmz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gvpkaugmr.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gofvohmmy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/galgofbnq.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gblvykjau.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gxcrnnwlc.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gfqfygxph.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gllfpphog.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gnzbfrxbp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/giovdmlya.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gdydnjdvb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gazsmhvmg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gweosexup.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gyflsckbr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gilgmjzxl.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gqvcrdeec.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gselufqzw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/glliysrlq.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/ggkapjybw.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gbuzajmhi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gozscgcty.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gpysdsdsd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gxwlsjpoy.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/geajcjydq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gacixvgvm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/guzksbygr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwaenlbgs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gcvadtsdd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/ggvgddztj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvypwhzch.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gvrgsbsmb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gnysqziqi.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gaamoljfx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gwcdpbbrn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gparfsphk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gfgcjkvjz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/ghlrzyoyg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gljkgxmjf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/ggqahkscm.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gxvrpphab.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gcysqijkz.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gbaqqocfv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gwusaevwh.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gwitdkddj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gyfddeieb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gdhpiqzej.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gjiclivwy.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gpvbaotzt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gifaudjps.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/glawrgeum.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gzfmagiov.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gjabdfpmw.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gusgsxtwt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gwezditpn.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gezblmsba.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/ghkrjcayb.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gsqzvtovl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gkfkkpyqz.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gaygdzimd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gdztayajo.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/glyluockh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gzlbcupza.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gvrdscqmc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gktelxyol.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gowzxhucz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gfybodzwp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gfpcryxkp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gezcimden.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gjshpwybt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gypjcjggc.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gsaenfrwu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gljgkcrjh.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gozbmcnbc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gfdpuuswd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/goyyplrht.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/ggwtraonq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gqwclrkps.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gfitvzccy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvnjefvko.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gxttzndul.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gejivmyzs.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gbtjupaxo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gwjsxpsyn.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gltwqbvyh.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/grjtrnbav.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gxdobdkpy.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gsijyyxiw.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gsicuakxs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/ghzwpqgnq.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gqgkkxaut.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gydzqsefa.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gunuqhval.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gnihfvfdi.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gxdmwnvxz.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gmuharnbm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gcjpsqgxk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gpdbkxmnx.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gkznsjuwx.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gzyjakqzu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gjsezpmrq.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gcypjedfe.sHtML


<!-- 参考信息 -->