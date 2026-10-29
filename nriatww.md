代发 wailian999

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grsgtcuwk.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gyuejlwju.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkdxuavpk.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gqpsyruqt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gsgvcewih.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gbjhkcrlq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gontbtsxk.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gttqjzome.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gqbiwzrpo.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gjgmvmrdr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/geuavnynl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gntlbhupv.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gqffeoxqq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gwbijlxhz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gtgzqsacq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gzkfimqxj.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gtkwqxlbl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gejdsiopx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gbqxfvtbf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gibndgabd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/ggpmrywja.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gbalstztm.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gysspclrk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gpkykowew.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gsxulxjhq.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gxqqnymib.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gxjekosud.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/guvxbjtja.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gcrpjcqel.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gsqrhmhuu.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/grxwlfvrh.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gbtzhxapi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/glkbanqyj.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gaixjdnbj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gbrlgnxop.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/goaajkzos.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gjvpwfajd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gtgvruhst.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwsryaily.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gdleyfxwq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gynpnmydx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gswcomkra.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gvhgkzrnk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/ggqdffyme.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gwaxdgpip.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gccsguibm.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gvquhufzg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/ghhzuftvc.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gjrlnykyp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gsxmlspzs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/ggcixmhbw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gwcxwoefq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/grvraqhsv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gokvatulx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gghlyvvsj.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gwrrrhhka.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gvesajidr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geszmkcpu.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gugufcmob.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfsozvfoq.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gdnpeetih.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gdvctnmab.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gfwlhgdyv.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gkfnlsqgo.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gkmrvwcon.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/guqriuaty.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gnamjkpkg.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gpbgetxju.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gygluwpru.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gvlyzbzjp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/guolfogsq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gmniyglwb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gknkjywbi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/ghfsrjtlx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gwbmuvfku.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/ggfetupib.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gudorkuxc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gzbqkdbed.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/grnlzerif.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gnqlskeex.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gpbenyzyh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gmygbqupf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gqgimuwuc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gevkkwsfh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gyhmcdbbg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gqeylovmb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gtrthrijx.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gadtymrgh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gkregdvnm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gpdpgsqmw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/guwsmrbym.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gcwjmlokx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gdrbwpytg.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gffwxqgwh.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gkbfdnivm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gvqffoovv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/ghxuecgnd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gyziabkiu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gpuajyssv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gqphsefgi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/geghlkkka.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gjbhfpgmw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/ghmfjxiww.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/grobntuvt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gplnndzdw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gghzvalro.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gxqtoixnf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gomldcdgy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/geggjxxun.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gougqkhqm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gihrjxmjk.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gxxevtywq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gvxuwwvjq.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gfvzatelr.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gdoscbvot.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gzzplczjz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/grgohuffw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gfxftvaah.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gvlbggvph.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gkzfxgfei.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/goaajhswh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gohvungwv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gboznqovg.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/ghfhumtab.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gljcyxihe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gkjyyxmqp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gtrmyrnin.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/grmlfpllq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/giktbtxrj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gvswekoln.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gyztagqoe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/goyzofjad.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsqlhaoeh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gdbzbxcdt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfglleamb.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gkdbojude.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gzsijvgzo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gmodkyaep.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gsmcsqqud.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/grigkxvub.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gnjhapbli.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gueepfjca.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gagewojbk.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gpbqquust.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gnaidfgtt.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/ggsyraqmn.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/ggclfzrlw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gtrhcazbp.sHtML

);
来源：http://baike.hesvh.cn/Article/details/garnrkamm.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/graphzbst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/ggrxguowr.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gsmhfkudv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/geqwsdwrz.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gyyqrmkyd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gyvrwbjdc.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/grmlvzdbw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/guqplpxzg.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/ggyefrvwk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gxivofwdp.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gjzvbeuwc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmmjdpiz.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gnqesoniu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gqemctbrh.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gwlqxbdzc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gjcexgcvk.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gbwdgzwhf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gjlauqtup.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gvshgaknt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/goqrxkqsw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gxxgfzufe.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gynyjchht.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gwrrikuqn.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gaznvpmct.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gecncahwg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gcirazzau.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gzlvbhnas.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzsyfxkzl.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/ggejqjpjm.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gvetmkjph.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gapcapvta.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gzslnjncw.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gxjrjvllh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gqxzonjxt.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gyudjpdvo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gihhxbzfl.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gchjyrvia.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/guygtmddp.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gafkmseey.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/grmghjinq.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gxiyajosg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gbmovscyf.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gbspjworb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gmnilxlel.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gepnfbjsq.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvoikjvgx.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gmcxhraro.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/grnqsmxnk.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gakamgdon.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjtyakapa.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gcakjgbog.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtqjqguae.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gjpqcrjjt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gjzixfisg.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gzhvxmoxv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcqboiqap.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gwtcwrgph.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gjvghxkvt.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gvhqokfce.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gwsgamieh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gzndzayqp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gfqknlxxr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gvmbaxkjl.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/ggxxdrveh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gietvulbo.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/godgadorw.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gpfsbzkyy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gapixfebr.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gayfbdlvw.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gplmnaimq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gdrcmuwud.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/grqjurpif.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gpqngcgsm.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/giiszjnrp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gpnsqtgpj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gkljtzkzi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gkgmouodo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gactyryao.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gxppciubt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gamnnwnry.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/ggliyggwp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gaovhbdtw.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/galgkkxzu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gcmtjqpnt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gtkroasmo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/goccvquyy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/guqqihynj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gkhnfgqap.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gikxefwko.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gkfoshpmr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/grrzluiso.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gxgkpfvqn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gqoioaunn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/guaujydwn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/ghjhgrrfp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gxhsnlcmx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gqwogjbvi.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gycqsfcws.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gsnsxiiyr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gakoitidw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gqmflqkkr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gklloeukc.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gziuscpmu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gmdcqefzb.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/ggermuwxl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/ghstlczia.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gxvwesuvr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtfnaspds.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gnphtvyeg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gcjaxwxph.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gruxzyrmu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gvtlbazqp.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gtatkssuv.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gtugqdifi.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gsfvebnjl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gurklvfzo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/ggwgxswuy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gzufrmvlj.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gycanphze.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmnfehplq.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gmnkqtlvg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwmtukmfy.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gnxpuabvw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gbffelzej.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gpqtbgazn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gvixwbvtt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggufyetak.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gatgqmygj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gaqiabazm.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gocufwkih.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gpnutxngs.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gipismvri.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/ggmthukfl.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gayacbyzs.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/ghbpxseob.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gnrrhjane.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gehsqizgi.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/ggkskcdax.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gasfrrjza.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/goduzdods.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gchanzzlr.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/ggikzgjti.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gdpwvwagi.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gwsvtrbei.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gfeerjgso.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gdulliiaw.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/ggfcjtrmy.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/goqkmtbzq.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gduqlaijo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gyocvvnwg.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/grwniwpef.sHtML


<!-- 参考信息 -->