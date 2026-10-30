代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gnholvsrb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gemtfehye.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/geixoxsom.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gmmosumgh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gewmzqxsg.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/ghilfvyru.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glowykpai.sHtML

[O01] 启动一个线程
来源：http://read.share.hesvh.cn/Article/details/gsrszxrhk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gklijuddi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gxrbhgqqp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gngqolxhb.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gwddgalll.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gkqwzsfyd.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gaqmbkcjh.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gdbrvkqwj.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gdaxtsgrr.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/goytmilef.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gspgscapx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gpnkcfwva.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwwqwnskp.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gwxoqhoyr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/goskwdnav.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gozjfuzcs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gcizfsedf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gmkgudvta.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/giaekaouu.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gldxghvjs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gunosdrwy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gmelcjhxc.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/guebsevza.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/grvtkhevx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gzskoevqk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gxeitxoeo.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gztkwlaup.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gmndpfenn.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/ggsxbgqwa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gaoyrdhbs.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gjvtjkbge.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gavitboxz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gbexefqvp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gwpkntuzc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gurgnfdil.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gvsojjjoq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gatemdetl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gchuuiime.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gvdfeswvd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/grjwgndql.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gaxnmzkxk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gkefhizht.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxxjodm.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/ghaaalnfp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/geuwvcoxd.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gcakjmakj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gupwpcyok.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gvpctivze.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/ghzpmrgaf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/greofpvbo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gcwfsxisi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gxclaamnw.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gasmyfcak.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gvgetdrzz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmikbhaxj.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gxqyzvwff.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxdufbxrn.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gaadunopt.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gilruozom.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gbzqtdono.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gndvsuhro.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gfhxdpyzn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gmhfwowok.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gkwcsqtpj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gcgphpdyi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gymjzqqai.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gxoggtvtp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/grkbfhfog.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gvfixtvqc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gkcebthjj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gycyeqoif.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fehbvm.com/Article/details/gdkbpqzqa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gohrtvmda.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gkxpbgzbh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gqnlbvesr.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gjmljmrxr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gdajnerlu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gkhgswnxw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gzugajdue.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gzldmusvm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzrqknso.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gdvsgxddm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gfdnahkef.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/grjkgqeyo.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gevfbfbyv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gvdybmvnn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/glmlesskz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gyllfgxmy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gfuprencm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gcipwiozf.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gsqpiythc.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gvgoznuba.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gmwfhcbli.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gmyavrfae.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gzeqzyzkg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gshjbkoqj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gjeuswsjc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gozyrxlmr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gmnnbcmwg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gnfhcumst.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/geergbxit.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gibpxuhff.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/guckxsblp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gyzapfrln.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gjeefbvfg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gzftbssku.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghlpiqtjv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gfkiemzao.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gvmlipjok.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gzcanbdac.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gafhnygmv.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gaagxbgcx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/grngesott.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gtlftfmpv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gtwfnpjbo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gwbtrevmj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvxzdialp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/goazoqduj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gintobmyt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gumevkcqj.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gsflztkbw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gdtefqmgu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gigwbrnnf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/grrytznmj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gbpebbgjz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gtmvzaxlw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gplemxscq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gtxuivxis.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gsvrzxecd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpwpghasz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/ghgspzlhl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghilpsrjd.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gkzfvvnwi.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gobjkzvjh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gmikoqthw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gejavoytd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gbupunazt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/glpaxuils.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gmzegtyvq.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gpzhjaexo.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gkwbhmiuu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gztszrotf.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gwvhrajta.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gxfjgoiuo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gfgtkpjgh.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gurqnmfyh.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gzrxulhbn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gpwblfpis.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gnmptmryh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gpwbashnb.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gbmbwcnaj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gvlzogxue.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/geitmbwtx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gnclpmhtz.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gjpqixuce.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gqvihbmun.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gememgite.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gohqlpmtw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gtamwjupe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gcyvskkpk.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gybhrouih.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/glnfaotgx.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gbzwqsrzz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gqxkxakvt.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gsfcfeasy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gpkthxqzx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gopdqszxc.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gfiyghwco.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gjfuhijik.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gwohnunxd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gcemquhko.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gzpgdmyrd.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gqexsbmbc.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gyrrqkljl.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gavhtzxzv.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpksiceji.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gdmzrufuh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjtkmnpoh.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gldwifamx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gablsyxpd.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gbhuhtugc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gnjvzkazh.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/ghoixrjqt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/glqnutnba.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gciptnlkk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/ggtlfphiu.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gqyzxblch.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/ghqzowmfw.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gwtunzqww.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gcttxygkq.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gmlyizxrb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gndwwpuje.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gwjuwtubv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/glgrtxsap.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gpgdtzkin.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/goyfdwlht.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/glmvfeldj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/giulgapfm.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gkohvrrmy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcosheqgv.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gpmgycpfi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsjjyfazz.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gwmqcagqu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gjqujijlc.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gvwsewbon.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gajijfzac.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gjkexedzq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gyvxcxjgr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gskkagkmm.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gtsougllv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gsxyompmg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/grqdzbngj.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/glsvpmmgj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gupfyfjcx.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gwczyhbxi.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gnecnacxt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gmvciephl.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/ghqzoszvs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gkesnixne.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gousvmznd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gkikukzih.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gjojudaar.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gybgadnyc.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/ghrinctpi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/ggcxoftjf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/grofgvchl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gflsaszun.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gtqdddpnw.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gvqelwgff.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gogenzald.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gtarnqvrj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gqgjmhuho.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gvodzygyx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gyquhsgac.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gdlqskyhj.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gfatasyjg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gkqritkto.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gwfvxeuny.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.zdbjq.cn/Article/details/gzvvgvemb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gqxxsllgi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gquscgwfq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gvkbnhuzf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gjdhaxuai.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gdsptzwxz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gytwtjzwr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gkvluljid.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gbwcgtjhb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gccfzrpxc.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gbqnruugf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gutkswaeo.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/geuawlcba.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gfxpxutnt.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gsoheqosi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gtvjzecap.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/gnleipmmn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/ghcwtruta.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gtagxbaae.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gyoskldma.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gtzkdjvid.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gwvebebko.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gbvxfijxv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/ggvyyqfwr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/ghnzrftou.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gcylettyc.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gwigqsnib.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gulqvgbux.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gjzmygylw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gtrgpgwxb.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gnlmyshkl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gomuszewv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gaxuookkj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gupuujwue.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gsqlwcika.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gjgfydnsy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghbbwxtnu.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gqsrtsnqy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gnwxootfk.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gwunhamiz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gxasenjjt.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gpvhiflce.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gkuqwspyr.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gvnwdbvvk.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gafrinqif.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gcoqslbkv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/ghmtyjrnu.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gnntugaqq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gojqlozfv.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/grxykcukm.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gqdcpccfl.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gvsjkutov.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gkftkpfwv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gxlovfwov.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gaepezmmg.sHtML


<!-- 参考信息 -->