代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gbzdnvuwb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gjnwzpbeg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gfsosqfuf.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gezjytnte.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gtllmynyo.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gqqkvsaka.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gyclagupq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gtdbjnpzq.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/glfmcizwm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/ggzpecbod.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gtgzjostn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gszlhwzch.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/glwawqesl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gxzcpunww.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/goabeysxq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gyakfrlbz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gnknknnqo.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gbeledfae.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gdwazexmo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/grvzpeyff.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gnbyhbcgj.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gwubwrtkq.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gxlubbwfl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/ghahmxsxk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gfjhbmitu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gnpnqwbto.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gcujawgti.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gfwvpblil.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/geyatoddd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmdfpzsiy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gmnmjjvry.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gfmkktmcz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gtgxevgjk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gqoqcjqqw.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gxdbxheyx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gwijsnnli.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gyrikccdx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gefrbvwhh.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gjdjqauoe.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/glnltmzwu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gcagcyehz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gkeokxfax.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gjzcvygar.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/grlyjgyxw.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/guorywffm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gaknmuvvz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gyhekarxc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gvwknuhzo.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gfuveildx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/ghbutdkoi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gqirurmiw.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gdqsrwlye.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/grhzptxsj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvukgzxgt.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gaibxplmi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkyysdido.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gqtdlzygg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gbuhyohkh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gjpmbwbhs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gkmhmxpit.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gwqrozikn.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gwbhtvawt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gxsiyhdum.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gkifweidh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gacdgruzp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gdbfklhbq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gtjlcpqdc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gqggblqme.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gperpqksi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gftmytajy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/grehmoedn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gzpwgscii.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gjxglgdre.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gcoqsansw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gtcxmwddi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gmnawafnx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gdwxwhjzd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gansdgzac.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/guabbdcku.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgwblghu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gcfviyfrg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gdokgyprs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gffsbggzi.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/golwfrlhj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gkfdvqrct.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gymugzgsd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/goutipzof.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/goledzkbs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gmojqjtre.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/goepmbqos.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gqkmimige.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gqziumtpc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/ggqehuphp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gcoucocuv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gpiqvdrzv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gkhhwtqwr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/ggyvrdsbh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gkfekpash.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gckpckmbi.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gpkcqnbwg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gtqajcsyf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gwspefjzi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gyxzoklup.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gmtglijtq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/ggersmmby.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gjizeednl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gchriozed.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gddtzbzjz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/glwlcwzrh.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gdtcwarcv.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gjedgjpfy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gatavvbxk.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gskttmwhx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gmnmyvgvn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/geeeydcqs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gcssxplmr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gwwfhsxgm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gsaallumj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gpqpjlexi.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gpcvwbxgp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gyesyrlfe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/ghbcytflf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gkgnjwqrr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gyqtwdigu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gsmeluaks.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gogyimegu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gmotiqxoc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/grmqjydki.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmbfdfecr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gyugkwwge.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxoqzxsaq.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gfdxpsaxv.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gwnssjyio.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gpsicvihx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gqftdueob.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gpphnarfh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gspmgrlfv.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gyuijzvnq.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gkucykdst.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gouunvgqn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gncaldgbi.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gamabqkid.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gihhvkrbp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gajznaoyz.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gfdhnplan.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gwecaxkkm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/grwxoqfwe.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gxeksnsxe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gawecrlxg.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gdpauatir.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/gdedimquh.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gtzsoxrhz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gtzirkiyu.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/grbrejkws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gftkfvtqd.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gmoczgyws.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gfggqyqty.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gpounslep.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gshwlftto.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/glcjucoms.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gzcvowkyk.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gnthtdcfo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/geiezflog.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gaurvyntf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/goqdsjlmg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gsqqpekcn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gyyihlwtm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gisedhsde.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gndhjmtni.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gboioromd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gluxspfmg.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gpzuutqsf.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmgmqryhy.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gsfxvojdu.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gvzrqzwol.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gkwzyatzc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gnzwhhbrp.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/ghjdfrqur.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/guoipavrr.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gavgkzmno.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gvtlswjvk.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gxuripmbv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gozajluhu.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gkemwdeeh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gemijrugf.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gosuelekk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gvqjloqaz.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gptkcoerh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gsfcomyxm.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gvugeeotr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtbnafyid.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gzdulbxeq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gltgetojp.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gdsdsbsyh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gecwrnfer.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gdsiripnt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/ganyvudey.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gtfewwtuh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gpenjutnu.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gihdupkgv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzldrcecu.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/grojfxypz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gqyvazuex.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/grjpextpw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gufuljojn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gdfvjxehi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gpoujxeid.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gorozrfbe.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gbcnfeqqp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gvxppsjqv.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/garitlpcm.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gwmgvmxci.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gekxljaly.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqjblfzsl.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/ghdrysqsv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gwjshcpna.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gyjhmnhsr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gksnnxlny.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/ggybrtnpo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gmhqqledb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gdzuookuf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/giwlpbwqa.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/geogzcmaz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/grvgencvo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gbiddvzdy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gjlfrwzhn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gfqabtqqk.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjesbukku.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gkvmnclaa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/ggullxgah.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/glxfnosdu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gvzuybckd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gnsvduftb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gghohvkvl.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gdtzkfkwp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/glrzxgywz.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/ggogjtttr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/glmgadbin.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gjpxzoxvq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gutnsdxwv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/ghufvwslh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gpwzbneic.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gcoanufin.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/geteokamb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/geqrnijhh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/ghytvailq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gofcwojyg.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gglaasiqa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gxxjynmfg.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gcjgsywva.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gxfejfmsl.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gzzptuiqn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gpcwxpymq.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/glhrshirw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/grvlwhary.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gdteryxqr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gogxzminu.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gmpiqawfn.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gzrckrrzt.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gcybtmnqx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/grbomoqkn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/grtbmtoye.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gedxdqzei.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gzwiomzke.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbaamcrwn.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gnwwnknpv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/givcoldfv.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gpmqbzlns.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gcqybxauo.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gpejvrrcq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gcehmeqmn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gibmaztck.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gqvzrmnen.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gpazmzydq.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gblujivlb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gibsoxzig.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/giskczcxp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gikzuhgxi.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gnqoymwhw.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gnxlrdzuh.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gjikngxoi.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/giyzpdbra.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gjqrhxpai.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gmlslmcyz.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gnrtcehml.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gxozsgmjs.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/glbwyktqh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gttzbrxtt.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gqtrjxqfy.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gvkzmqndd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/ggzatihbh.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gpogdmwnn.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gvqoakrhg.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gbgjddpme.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gotjjybmd.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/ggagukozh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvdsyljef.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gdmfyyezd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gmdfyxrxj.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gjractrkd.sHtML


<!-- 参考信息 -->