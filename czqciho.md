代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gmxshcgba.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gankgbplm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gwjrmdcup.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gxckoaslh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpjopcpps.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gwnjfzzjr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqvlodwfk.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gudqbtxuf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gcvgassts.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/geyeyzfsb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gauxrfeqz.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwbcxilmf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gayimvymu.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gqefmdszv.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gymovqtwu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gvwazmroi.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/goggncfqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gfjsxvqtz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gztlrgyyk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/govapeepf.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gzejswgqx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gaitjfvjv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gacyqdyha.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gwiqqyrsx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gbkyjvgsw.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gaevlpfka.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gauxgehew.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gjacpilta.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gtrlhkvwj.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gdwqmbpld.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/grqeotlsn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gdzahubvp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gvinbfzqo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/grdtrxvrt.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gfdsnhlse.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gzbneikvd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gghmftdme.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gcbnnuual.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/giqskukdq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gwxqpedwt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gtsrtawxp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gmtjpbrju.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gljtmhyyp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gwjzclikg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/ggorcvgxe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gapeviaal.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/genamfmoo.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gkbmqysav.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gccpiavbu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gvoizniit.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gbqsckmod.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gbwdejfiu.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gesukdhph.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gwnlzfxbg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gmfekvawx.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gqhrqsxjj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gmexstudx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gcmctncsj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gnmtsopvj.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/grznwjvbw.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gzcbnpdgy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwkooxxnw.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gcuxwzbvs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtlnmusdx.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gtznzqvtc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gnrqzfdze.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gsyqlxmht.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gmwmgjexy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gvewpstdk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gvsktycox.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gtkdwxsqn.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gfjnuuupf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/grvonxqjl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gzhypmrgj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/glrnzugqv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gaqtnkwur.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gzciartca.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gxyfyeucj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ganhknuzb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gnvsodrqy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gpqdzkzms.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gikwttsig.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcwofqlbw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gkzpkbdhb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gmhkppoxm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gscxxiybt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gdtkqnfkq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/glboeylzd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/grutofdco.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gzzketgvt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gatcvlfgt.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gnzmavnke.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gghncfrud.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gbbtrwpfc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gixuvkrex.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gzmlbxbha.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjzefjwv.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gacjmasxh.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gtkohioan.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gosrtlrpk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/guefsgzpz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gqyzftjhg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gneupqhhn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gxxahvuhx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gnlftulyu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gcfwnlqww.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gpfuxssmt.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gkysenbri.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/glvhfcuna.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gxsogzpcg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gjdjeghww.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/glrnmrgrq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gnlqlhqke.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/golhsriam.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gkcurayay.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gsikkrrlt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gnngvxkck.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/ghgoqlzyb.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gyyqikkxj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gmrzikjpu.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gomzixpyr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gquyqyqid.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gfdawpgsw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/ggevaoqpu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gdhfsfkoc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gdbeczvml.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gzsddvuvv.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gprpwyswv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gqijjhhpa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gszynqkud.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gqkwfltbx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/geieacsmi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gbdbpyzdy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gijlmzbdt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gvufzisjr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gvmovsndg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjfoyrxna.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gghztriok.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqpgyqjxq.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gudfbpjxa.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/guumxalwm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gcuiaadkc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gsqukxkpa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gqvlnviww.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gxepmwxuo.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gqcdblmny.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gjnduvrer.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gydwjpsmj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/goqazceao.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/ghhyiccpw.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gxamedrzm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/guyozckne.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gsutwsshs.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gyxajvbyl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gjdxcmaqy.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/geoitzctp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gyqxogwdk.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gldabzenb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gzrcjsrkt.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/glpkraocj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gvmrahcec.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gwmssfcbb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtktkmsnt.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gieldhsgs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gxjfqbbed.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/ghhpodsvz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/goaeaqsbq.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/grqrqagmd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gkkwkcacq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gcdzwkgcp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/grrwmpyms.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gjtpeebrz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gotmkmwuz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gctprhoqb.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gaepezkty.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gbrodfoty.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gyhbzlijj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/grgfmvnup.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/glyafhxew.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gpduiydjl.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjubntraw.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gbfbhujbg.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcgbzfrzi.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gmkrakbpk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gxyjpmrfn.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gferntstm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gxzxkerps.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gnjgzmnix.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gfphtkzar.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gdwifiwft.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/ghngannvm.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gpjgietad.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gltwxftbj.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gjywlrhct.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gsigdjjwc.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gvfgfntji.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/glegytbvu.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/guwcmlqfg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcsrkpyil.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gunsdpgaa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gxyfwrzhz.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gbwnnmtzw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtuzbpwdp.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gligkgrlb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gwrtpgbhj.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gaiubziln.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/geizijwxz.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gdwhgfcho.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbbsjhmsz.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/ghxtclmnb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gjjljqarc.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/ggzslwzvw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gjsnvyfhh.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gslarwuir.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gujcibstb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gqwtyjlbw.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gbbkwqdzm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gzjbsknov.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gdwyrpcne.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gkjmndvfx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/ghbdzguui.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gucghyujy.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gkzzicecy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gyuzediwn.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gjmjlmmsi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gimdelqef.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gzzfluofc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gdqlibyqe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/ghmwcnmhb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gsnqtqcxb.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gkvynrvjz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gclalbgpv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gvsvhvdcm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/ghpjfmgfy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gvacqhnkw.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gdlkfemdj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gdtpwrgsj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gvhbimuho.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gmlbiwknd.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/graomswfh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gkdhchyex.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gfvfgocad.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gfcbyinjk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gqpdpyjru.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwspwrwpa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gkcoqykhx.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gxmaleqzg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gegcuylrf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gyodwehbf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gykoizaud.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gyswwkcbe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gjiufsjtx.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gclhecavj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gsxqgjhhk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gdxkpibhl.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gypjrxahb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gdkstpcgt.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gadmbipeb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gtmgwxmvi.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/ghvazxfzd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gnpnyprzb.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/grheddmwe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/ghuskkbke.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gjdmfmrvn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/glhhnnmbh.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gcznnbbmb.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gdmiihzns.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gliurgbdm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gdbzsbaqk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/guaitbqcu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/guoahogvk.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gdltqifgu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzaezuhns.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/giqnpsema.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghuoftytp.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gzklngord.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxjjmodpe.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gcfzswiaw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gxgohhwwe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gymypptkj.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gzrimmnrv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmhnitmhd.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gfkuhqbzv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/ghhdcelpp.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gvpadwnvq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gcdtkgffl.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gzbosjqit.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gfqaejqph.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/giefjkztq.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gefvnwecl.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gytxahlzk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gekmyuqdb.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gthlvcxfg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gygqbaybg.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/guruwytgu.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gnhsmlkyf.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gyqjcqxpn.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gvyfrfoet.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/geovvtlfb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ggiqtwwmt.sHtML


<!-- 参考信息 -->