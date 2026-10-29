代发 wailian999

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxxfkabdn.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gajqdopzs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvegbijxa.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gadsbceuv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gpthseubr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/ghaqvmpoa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gonhosfcp.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/grrzazgzp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gsfqbllob.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gwpgknwrb.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/ghrcigbgl.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/ghswvbqdq.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gdykkwgrh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/ghwhubbkf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gjfkeitgl.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gmrznmada.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/ghrhjlyfm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gikuatnlw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/goukqfvpa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gglwmhrqx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gxcegzykl.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gikgaejal.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gnzfyvsfw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/giubzpuxh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gvrxknmgf.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gfxhzgkgl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gkhjrnnqp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gkpyjsxyz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gzpulgbyq.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gwyueuqgn.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gemhpaexr.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gdvexvirx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gwpabqeyg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gwmkbuxhl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gaicmlbnw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gbwyucdug.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gdfpbtqfx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gwnjbwtaf.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gpjqhmglk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gcxadndqm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gninikynp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gxrmapnxy.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gaxdasbbt.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gdbratfvs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gcbohhgyc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gozvsonmi.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gvtfamqqj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gwzdimvyf.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gfmvtnszk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gcqimrhbp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gxnnpankt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gargpmclj.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gpyikhmqt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gtcypbaaa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gbckywqiz.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gwfdkhrei.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/glgheafgv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjaedxnvl.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gdkouaedk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guezslvbz.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gyjhnrukb.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gkubfzfwy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gshcnzuhr.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ggtwmhdzr.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gfbiiezas.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gcfammfyl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gzqigqmvd.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gqpzkpsyn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/ghjhjhtls.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/ggtcsdsca.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gocgvvzyk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdlqhpoia.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gxaybeyqu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/ghpxtaugg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gmjdbkowy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gcgicyiva.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gyskixfno.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gdwiyixkk.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gzciazpjl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/gdfbuwceg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gjpfhogxz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gwcjstepm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gasjhzgfe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gwocyffth.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gagbtuwoy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gtuysperp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gnyvojzze.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gpzfhfrfl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gfdatfgxw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gafymcyox.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/ggbqboiyo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gtntmnxvw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/gepmiiooj.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gccpshzvz.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gsfdlhmqr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/grcnnwwnn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/ggdqzgznc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gxalhruxq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/glaiptwas.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gqyzmsyuc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gzzwhrzux.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/ghyiavbsi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gdjyqfkku.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/ghoeodijl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gcxzpkvak.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gdinscpgb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gcwuygsgm.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gbbhzdjpn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gzdlzglrd.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gbhszeepl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gznnkfhds.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gwflxvlvt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gusuwpisd.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gzltbkpmb.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gitzowprh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gqurpnegb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gywaorglu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gtshmlsxg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gnajmhlsg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gltbemzdl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/glcovxljn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gpcrbsvby.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/grgxromaq.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gxefnyjfh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gbiptgryt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gajiewzhi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gjkhbnqyh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gercwlmsz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gscmfjufu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/ggwvstayg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gdnglvtah.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gccrqrgwd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjdmcltbw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gnrwxsekw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gemapmimg.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gcpbbfaqd.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gkcyofilg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gwigzdwrl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gdccqhwzp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/glnjulnmj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/glzwutsag.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gvberhsqn.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gqqqqeegm.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gbmfnzmvu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gtpmwpxkd.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/geohfxhdu.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gvjseslev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gedmjyjka.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gdoumbrnt.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gioxeiznp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/gpktqkrkn.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gpebaqysg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gzxwymjpn.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gwfvdpbbv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gkhmkbnmy.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gblhnxmud.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gigtfrdtf.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gzggfdwdf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ggafsbmdo.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/glewoturp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gyuljhsmj.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gdimhpkjw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gbmyicmhi.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gjimuxuhs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gjhtlacar.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/goajalpcn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gsixkjpjh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gwnazplzr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gfffqigvd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gjedkfcix.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/grchwmkyq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/grvdbgvoc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gphitfnto.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gazfigxdc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gfelaqaai.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gtsjlhrbu.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfnwkamdl.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gdjqwpgkv.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gxgpayepx.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gjbdjnzwu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gqdxyuzxr.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gldwkxrdr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gdsxkvbmw.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gcgbpwjek.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/guubyspbq.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gwkcrmrgg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfrxbczdr.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gfifevbdd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gflqtqewz.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/ggnmtfjoy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gkleyzort.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gejqmllws.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gcrmjnlly.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gyfjwbyse.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gevzmrvkf.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gtggwnwow.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gtuiwrjdi.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gcwvdxgfk.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gydtbcujw.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/giyxuhsic.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gkwwemctg.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gcktswtmw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/giyzmfmnz.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gacfvubht.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpeinsnxo.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gavaqfjfr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gdpaafnod.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/golsvrmde.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gamlbfuyu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/giqwdrxpi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gojpnmxvz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/guycsjamq.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gxwpvfxak.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gnaekzudu.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gsidweiji.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gxvppwqvc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gcsffuhhp.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gszmynlok.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/giqedkhop.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gqtizivjg.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gyitccggy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gtylppehg.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/grmoctjuy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gxkqvuhzi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gfpofsbgo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gaqbamjeg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gekadxnhu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gfponlrsk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/glspcxirk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gxnlrlhsv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gzeojxdlr.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/grszocsje.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/glwsovmrb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gdkiffugn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gnkfuabgi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gdxrkcdqv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/ghuluzwfg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/glxptnfme.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gujftrikx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gkusxmaaz.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gaxrskalf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gosntablo.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gxhzbbxlo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gaftnblpv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/ghgwgjhuu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gtoqzimmw.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/grrgasqis.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gidyhdyok.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/ggifhjrrf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gjkhqdofi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gxmewmhar.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gjpgddboe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gofrjxiip.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/guqwpyzsp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gyciyenfm.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/glyhuldyj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/genqsmxvd.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gjyfhtxev.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/glgzxxisr.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gharkfgzi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gshlslsmt.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/giziekill.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/grwinzaeh.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/geyhnkfoo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gxbsnghem.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gxbwtlmkm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gftxmojsr.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gxbxpxhyp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwrdrvdfz.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/glrgvqsfl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxzkbczzk.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gqdifzgih.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpymhpmdi.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gxzlxnsvr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gcbbyljtk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gimljkwvk.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gmafvnlom.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxolhjlyh.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gdxbmmrbb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gaeanacwr.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gyfebqdtw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/grxxwkjcz.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gabevxtkh.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gxlhynqif.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gvcsbrtsx.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gkxgchlud.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gxuupefik.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gwpgbnwdd.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gnhjpnqab.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gdvsabwbs.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gwgqnrlub.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gkjgfpgxp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gvgzkyygz.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/glgshsknx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/ghvqgpyln.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gccakcnoc.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gwdvuzmew.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gzzywvpzb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gwedbqiwe.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gkuusfxhp.sHtML


<!-- 参考信息 -->