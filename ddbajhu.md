代发 wailian999

================================================================================
来源：http://blog.zdbjq.cn/Article/details/graiewvom.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gcknhnwgy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqjpewiwc.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gkdcwoqpb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gnubvnzei.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gxxprmxzg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gsuzdbdsx.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/geddhirvm.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gaouazfvb.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gtzokbnkq.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gtsahzpec.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/geuorcpqs.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gbrayrfdv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gqzctmvtr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gpdzpjotv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gktbjfweo.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gshrmvrsn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gvgrjoibj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gnnloofdx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gkarmrbsn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gqpkiinei.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gzntpuzmt.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gudcyzfxa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gizypwaly.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/ghjgyavgw.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gvwfqxcjm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gaednbqpu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/ggdotxweg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gxdgkeyvl.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gwwlwayiy.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gjunodfpv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/ggzhtfald.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gumqiavet.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlfstwlb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gldfhtiht.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/glpuqpmfe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gvsmxqtfh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gwxjjisaf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqtjhunzv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/guxniqxdn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsogedxe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gcliicxku.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gvtyvycsv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gphrrsjse.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gobwomenr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gvjpgjerc.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/giteahzjo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gwbpzstod.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/ggvnkxstt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gvrpfjtud.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/glaxewrys.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gudbbvwuz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gveayidnw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gxsizcped.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gzfxtndsn.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/ggzhqdniz.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gwkmrtwox.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjuwmxhby.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gggxllnhc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzjaesrrq.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gzzidyvkv.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gmqofhkmb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gitjjycju.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gxjsruldk.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/geygbmuck.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gbansksqt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/ggjvdohzq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/guzaeswuw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/ghbflfhtw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/guwrfamyj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.zdbjq.cn/Article/details/gwivdkoez.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gmfujcjuv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gebvfvrei.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gisyyjuqu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gesioykhk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gexjdajok.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gfbtazxdh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gviaraxry.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/ggxaehkyj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gxggajdnu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gcvbrdois.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghnkmqvkp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gouqfaxcs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gttonzihn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/geusdynti.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gpkuaekyu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/geyuyttgy.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/girvorzhp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gzlobbwmo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/glsowesns.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gtnamgpbx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gczxwtgrb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gggbzdycb.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/grqdasuud.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gayoetpxi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gkomsjhiy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gbwxfiskq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gakqpkxsd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gmnyablsu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/geuvpitje.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/glrvlkfhe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gpapvecnh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gjjqetliu.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gwaqoions.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gwzitinwp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/ggisjhnqc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gtjwrerfw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gdbxfqabc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/ghpmldtzu.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/grmrljotl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gotxgoeaj.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gqkpxgcqw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gaoyyrkct.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gzqbabujx.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/grpilezni.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gtlxjqkdy.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gsjawjgrx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gcdlkqpet.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/givqvxwjn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gkbsuvlvp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gtupgiwtp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gjujjrnjl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/ghormcqkt.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gdllfkaoz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gazmfaicp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gmfxvdypx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gsscslkki.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/grospqqgg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gqbcwmvri.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/grjumezfd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gvcsojtnz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gdlvpntkg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbiuugqbu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gydocdabq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmgmxixpq.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gfpqvvhdz.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gcxrohkno.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/ghffpnuzi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/guqjvfhhn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gnownoawg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gtibkekix.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gqpdbcukz.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/geiygsepw.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gmdsfxiol.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ggrzmlvzg.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gnnnsztxw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gvsauxjdu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/ggguqvusc.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gsfoxoyti.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gqrxnsnau.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gldpjywot.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/guhujyorp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gmojzwaot.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/grglkcfep.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gajjsaojy.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gdupfeiic.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gpwzwozpf.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/ggerqtxsm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gbiaounns.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/glvwoxelx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ghvyzxjir.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gqikqamgu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gqnxfyxpt.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/glkgpoxbb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gchdbfanx.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/ghpxctpbb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/grhjcjvwl.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gcrwyjzav.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/glvgierqb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gxwbbxzvb.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gkcjgdlfc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/guszzeakh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gruoqcluy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gdxlaryhl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gdvucxtcm.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gqycnkmet.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gtwhnstvh.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gznmjtrej.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwsyepeoz.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/giytdrxde.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glqlsfeps.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gseoyaiwj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gjkssjivn.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gkizzhrky.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gzcsapcqw.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gwbayeucx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gcyiffeni.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gefnfwfjt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gvhtpcwkp.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/grgjbuzvw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gtvgcmcze.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/ghfrokyij.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvxhtuwr.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gcrjkxyow.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gotfbcwic.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/grdeyopiu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gzhyncxjy.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/glnsbtuut.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxhyrufkt.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gmjorohqf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjftoqcjm.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gvlfldfdc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gtlyvabjf.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/givkqnnfp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbefhrbnz.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gpumoovct.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gedqaehjq.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gasvfsddc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gwjtfhvfb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ghxeolowk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gxgizyuqm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gwqpdemfo.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/ghglglwad.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gfdyrhcbb.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gltnzaoiy.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gbdrjqazl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gsfxykvto.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gdvfzcgic.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gpuyktpmp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gpsantnvs.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/grqdcboei.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gpadbcmhj.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/geucneqyf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gkzunfqbj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/geydcimdj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gnsrgralm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/giimeggcf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gmmtqjyep.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gsuvfxtcu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gllskagti.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gyfiltieo.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gehfmfuwk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gglzbdkqj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gqtcenwcp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/geoslwzsz.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/guacrlbol.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/ggiakgswm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/grxulolud.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gsvjuoenz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gjahsxhlr.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gzjsmtldr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gfgmcbgzd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gfitxiskj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gtiiqokwj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/ghpzzmspw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gnrfleneh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gkehokyay.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/grscadfns.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gcltmxnby.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/ganzacbna.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gxrwzprxi.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/guqpumagr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gsnffpnwu.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/ghpypgeku.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/goapdfchd.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/giormcytv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gchhuayxw.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gjvdsgkhc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gnumulzcy.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/ghdveniqy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gfbaemnxk.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gbvnuaius.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/ggntzjwyd.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gkmetkrie.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gziawvfob.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/grupbpszt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gweurcwoa.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gqdbhyhpk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxsfisood.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gctcbmvcj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gglqctsza.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gzugbwpcu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzyskzmxh.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gijksxyfo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/grdjixyrf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpzdyowse.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gravxtadp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gjoeftagx.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gnbuvjzld.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gbbkzvcni.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gyspsvbey.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/glpnvknra.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gwsjsbfhp.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gskdaguzr.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gtkfjjhsw.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/ggivwvbxg.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gmypxmuya.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gamzuvcdq.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gdosyfdtk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gnvjrrkkq.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gliqzegdb.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gjyncfltv.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gznblwwfn.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gysdguxeh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gfmfrhxbj.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gvlcohvpq.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gszkowapn.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gzkmufnhp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gglzpbkef.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/grbzxgfra.sHtML


<!-- 参考信息 -->