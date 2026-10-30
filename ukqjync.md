代发 wailian999

[O02] 使用线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzvohtlu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdkeghsg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvozmord.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gfvrynads.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gfefxhwzx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/ginsszeyw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/gelkkymdz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gpaflsryd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fanxiaobao.xyz/Article/details/gybekphqw.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbosinwrg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/grwafzcmq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fanxiaobao.xyz/Article/details/goolgnbsq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fanxiaobao.xyz/Article/details/gkrfkilit.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/ghslkcnje.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnnjfxbf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxebcvavb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gbmcoblbo.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgyfiawx.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbdbwuca.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fanxiaobao.xyz/Article/details/gomcxfswn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/gxhioujtf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkfqqznv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/glerpaibl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gpafutdhi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqnulxbw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fanxiaobao.xyz/Article/details/gltslvdyj.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjmyrqdp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfodilpo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gwipfaxhe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwifkxiv.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/glgsiytgc.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fanxiaobao.xyz/Article/details/ggfynjusk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaseidja.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/gaqookyyz.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/grznwcrtq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpedouwl.sHtML

[O06] 使用进程池
来源：http://baike.fanxiaobao.xyz/Article/details/gvwaagkjy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjpskpxt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fanxiaobao.xyz/Article/details/gdbapobfa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkywvcbe.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuqowbfq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gfurytixz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwjndkhv.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/glmycucuv.sHtML

C#:   Parallel.For
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gainxvchn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcswrrhrl.sHtML

P. 常用工具函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpswzzeg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfisvtjqa.sHtML

[P01] 生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/guqgpiszr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbopucfh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnqnmpuk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvurrsiot.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkdrwxzi.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gxlnyephw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxxtcjnj.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gsqylofjo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzjjskjn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgwrwatb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrbrmjnt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gkgofhhkq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/gybdbyouf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fanxiaobao.xyz/Article/details/gsehsuqcq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggypnwycq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fanxiaobao.xyz/Article/details/gndaetgrp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/geyablcsg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fanxiaobao.xyz/Article/details/gciavnwgx.sHtML

[P03] 生成短随机字符串
来源：http://3g.fanxiaobao.xyz/Article/details/govmncdvg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsutdtyt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fanxiaobao.xyz/Article/details/gqbxrmbtn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gurnovllk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuuyaxsf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfgzgqlh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fanxiaobao.xyz/Article/details/gxgmvlgfg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fanxiaobao.xyz/Article/details/gjsxazqnk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnecklgb.sHtML

[P04] 求长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqgvyvihf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogyxhlgx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcwcurhr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fanxiaobao.xyz/Article/details/genqdvtel.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/glgisnyow.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuydmqli.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqkqyoog.sHtML

Ruby: x.length;  x.size
来源：http://baike.fanxiaobao.xyz/Article/details/ggjclpgzi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gzsomnlju.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnrhibrr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgnvwcpm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtezwgxyb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fanxiaobao.xyz/Article/details/gaovapcin.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gakvanoxx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdlvzird.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrmkkhqk.sHtML

Ruby: a == b
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqwatgsu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtdqsvmh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtokozcxw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvfzbyof.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcrugbly.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fanxiaobao.xyz/Article/details/goxcjhmgd.sHtML

TS:   if (x == null) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqovllvb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnbclahez.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/geepqrfhn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fanxiaobao.xyz/Article/details/gjsebyvpd.sHtML

C#:   if (x is null) {}
来源：http://3g.fanxiaobao.xyz/Article/details/grohdhseb.sHtML

[P07] 防抖与节流
来源：http://baike.fanxiaobao.xyz/Article/details/gwebizbny.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxdvtjdt.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gnsmypkhw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjuzxxpf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gahdhihnq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnbmmoom.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fanxiaobao.xyz/Article/details/godeavose.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gherdptnm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fanxiaobao.xyz/Article/details/gbkoqhozw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fanxiaobao.xyz/Article/details/gvbzwogvp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gnuvwrfsq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gmhljjktb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fanxiaobao.xyz/Article/details/gghzirakt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gyoczkvcm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fanxiaobao.xyz/Article/details/gcesuwgug.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgsstugw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjwjfhoq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fanxiaobao.xyz/Article/details/glymipjon.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcnzhrdqa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwvughtf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwyvwgxb.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwznvvnis.sHtML

CREATE TABLE users (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcouyltwp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gkevovsle.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgyirdsq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fanxiaobao.xyz/Article/details/gqzvbpdou.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fanxiaobao.xyz/Article/details/gmkjfvtio.sHtML

);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaufrtjzl.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fanxiaobao.xyz/Article/details/godjwuuvl.sHtML

CREATE TABLE orders (
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhteyfzn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fanxiaobao.xyz/Article/details/gktxvqath.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gqajzarwz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gzpoesypi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gcpnbqmec.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdbbifcx.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/grhqtmgta.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigczbum.sHtML

[Q04] 修改列类型
来源：http://3g.fanxiaobao.xyz/Article/details/gmvdljivt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/grxrlrihj.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gjjnckrwt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdigzwok.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/gjcduygmd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlnruegm.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/gflxfslkl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqjghhxz.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gdjwjohos.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsjhvwmq.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fanxiaobao.xyz/Article/details/glqvmixht.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgnmytqn.sHtML

[Q10] 插入单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gworixfck.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gebdcljwh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblhfzupt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gtupneaxh.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fanxiaobao.xyz/Article/details/gguagjxld.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fanxiaobao.xyz/Article/details/guyhdsqfs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gohfylgaw.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmgkuebv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/ggmgweorw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjbrcoka.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiehdiav.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gccxiowgv.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/gmomrmepr.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gedqxdffy.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpkyzmdo.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gziwibhpd.sHtML

[Q17] 条件查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqewzaosc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gixkaoban.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ggogrxlgr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqwmyblm.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtjvokrj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fanxiaobao.xyz/Article/details/gqklkcyxz.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/ghajjbcri.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gryqjpxwz.sHtML

[Q21] 空值判断
来源：http://blog.fanxiaobao.xyz/Article/details/gvsimoday.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwkzfkds.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqucfahsr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fanxiaobao.xyz/Article/details/gzngfszfd.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/goxfbjobf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgfquxuf.sHtML

[Q24] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqrrdgnz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnywnlst.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/gunxsscls.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gdqbxqwgh.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gefiflktf.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gqkzqjihl.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/ggenyydjk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmoqghsey.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzkpgufg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuqleauq.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqqwjfbj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ggupflmhp.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gcthtjuvh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gayigpuys.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowscvoqi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gxijtygda.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsynoryi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqathyew.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gmixoadml.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkxjqsqj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gdeorstvd.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/godzmosfp.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gxtwjofmx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gaidenwof.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoyssizg.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gcqkxrrcw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gknuduszp.sHtML

[Q36] 左连接
来源：http://3g.fanxiaobao.xyz/Article/details/gzkrxlfhk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gktszradr.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmplngox.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/garpwauva.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/grdenqvsq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gjwulqdib.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqkszpwy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxkxzezy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsbpmnbd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfnvdnte.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/goxwlyyel.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gvzqaibzi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gqblfzein.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpyeutsp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gkffvirjy.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gatxhilqf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydktzyif.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ggwkdusao.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/govarjhsc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpytsnbop.sHtML

[Q44] IN 子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gxosxowoq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmkdeqzr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgrxzhoe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvarhyuk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/ghauqzwna.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxemkbtv.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gukubthgc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjioulbit.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/geipimwcw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyticcye.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gdkdgmvps.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gnaoqdalw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbfvusts.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gldzktrum.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gtrocgmdo.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gcjtttsdc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauexfvhe.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gnkdplqxw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gqheyuvga.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gseiihuxe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwrttsgx.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gtkdaukrw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gzuwqipal.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gyipplmhi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwmhexuh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqtvsnqa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gheyxgoqe.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjnapudnq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gjupoqonp.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gevclhqlh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebejfkvi.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmqxxvdg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaodexuv.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gvprmbeuk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gsvevssax.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gaeytzhiy.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gzyiqgyya.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxbcwifx.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlenmmbe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxpaogye.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdevafpj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzszswkzg.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/goupcnplu.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gdraqttsb.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gldbxuvha.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/glvmidzau.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giauhqhsb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gyctochzm.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqapgdev.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfrsjolv.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkvuneqm.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqxllhnbj.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdzwwxha.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gguquhlus.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gyxafpsuu.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gewrexuau.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxmgynol.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gldyfflub.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftiluhuf.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvicypzai.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gluhmuegr.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gfwatqpsb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfinvvhf.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjiyglwu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgxrdvah.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/guxmfjmvr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjyfctxa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexioumiz.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gfszsenvv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/godexjcxf.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/ghfscbzop.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gvvydqldu.sHtML


<!-- 参考信息 -->