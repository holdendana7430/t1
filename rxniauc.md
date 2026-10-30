代发 wailian999

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzozrjlyg.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gjeoevnoa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkjvjljcu.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/grskgyuzs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gauudhzrm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gldidnriw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gnehuwaom.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gbkbtdecs.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gbgdxljbr.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gvppdngfn.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gktcbgzvi.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gmpxgkylw.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gzsaavyvq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gmlcjpmwv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gvglotzdj.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gtytnabwe.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gldtefoxb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdgcxvxi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gruyjrvzs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gpenfzush.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/grpsjwdpn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/giyflooph.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gcuunieaq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gcwynnwfk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gzczkwatg.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/ggifkbdbw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gjmjoyhxc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gxixilubu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gmzvraacy.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/goxfrpneq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gqtxhuxhy.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gxnxtufqp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gfzkcbepw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gsgrnejsv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gsfkuyjxx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/goybxpqiz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gcdgejqlx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gnuqkwmmf.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gfoetuagx.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gclnysycw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gekvqugqs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gtzyyxget.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/grblrrerz.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gmvioslix.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gfmahrzuz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gmiwqiwti.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gtctakhfy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gexcgqscn.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gjfswzgog.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gwooficdr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzcbqmibf.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gtczlsryb.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gxicftlzf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/ggkxlsznq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/ghuddhvxv.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gmphldpsi.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gewbjqkxs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtfsuumqi.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/ggkjgjwgl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggoabsmkc.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/ghjvkeald.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gbjsbmclv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gnltalrgu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/ggehftllm.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gnlophfqd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gbulglczc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/galewwfho.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/guzctptsd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/guledexgx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gjhedcptl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gpdbzmlav.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbsuwenwe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/ggkylunqr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/galizihis.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gpzprtcdq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gzsprrogo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gjfnfphee.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gmesikexa.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/gqhhcicrv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gtubxltla.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gvhkqpxpu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gamgvalen.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gixrruhto.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/guuuybrhr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gwxxokema.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gyqbhfyay.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/grdlzdcad.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/ggkxxqvrh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gqtxsruhb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gkrpcyfvi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gzeuxmfwp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gygaltfmt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gwzjndaam.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gauzviint.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gmsdhgyxg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/guybpskwe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gaiyafnow.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gsjbkwhqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gyvfhpnxn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/glfajqsqw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gtnyildmz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gmemtinnb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/giaaritff.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gqfngofju.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gkcwbojrd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gqzglokpl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gubuxwtsd.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gcyuqpsfy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/glpumidrv.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gcnydvgkp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/guzadetfb.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gdzjhgmjr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gtmewkkto.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gxtaefkal.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gyhbifdjs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gscibkmzg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gbnehvsos.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/ginbpieek.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gdrmwgdfo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/glkowslgu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gqjaexehq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/gcaqepncf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gjnzvwqzc.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gruiemruq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gwmpzrzsq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gqaaapqjl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gnqispqxl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/grfwvdcee.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gzzfschdx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gbvymgzxb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gpogzopdl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gidhyjjvr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpjarcgne.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/giriczkgy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnmmevfhj.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gdarhfoac.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gsclfkxuy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gvntslmwf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gtkexvwxs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gbmslosts.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gzgeflfib.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gjckjyiqp.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gdcgdzbun.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gyknpvycf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gjkbsysvs.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gfmyetdxl.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gsdjocpwt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gmenmuxfv.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/guzvidyan.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gluyhsamb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gnuotfagq.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gtvvydcwx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gluplqkwk.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gkpyehxfh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gqdnkuwhy.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/goumumgoz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/goxqnnfod.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gxazrneqb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gfutbocxn.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/gyrqjvzlk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gvinefoek.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gtfwicqzg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gouschlkr.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gsuzsodqp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gxxmmjkup.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gzerqbrjl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gkuoeewph.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/gaivwxgky.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/ggjiossqe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/ggqpfxauu.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gkpqwvyxl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gxcydgqcs.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gtxuvqouo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gnonxfyll.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gslxfzptg.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/greweshxo.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gynpkukcu.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gyhiiwwvb.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gfdsxislq.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gghomnoqt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/ghqtxrrid.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gxorakyxu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gexwyaxvd.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gzxcnbruu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gkftahgvq.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gxrarekim.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gvxjtdajq.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gbuaxtsyr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gtktgnlro.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/glbzykggz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gxpfrpvhc.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gomqnxdha.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gmquwfvor.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gtprjbdbm.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gexvokmap.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gllthalwx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/ghblispsc.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/guhpnvjiy.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbtlwmevq.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gjyydoqbc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjakafdbh.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gerqhtdrt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gatguzowk.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gtfajwatz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/guafjjvvj.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gnzmgkwaf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gqoqmcsou.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gypbnicyn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gffoxsaac.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyksyivas.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gyzlknmvk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gwpysccxf.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gymxmcado.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gzhxkictj.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gjsbpvvuh.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gxvwubqjx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gdzlhacla.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/guhgvivjc.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gjfjqvjhy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gpaxizizh.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gykztspuh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/ghymaaliv.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gomimssiq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gmertwnwe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gszaqdorr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/grseehnge.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gkmhmznfe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/grjllyslg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gdsecbqus.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gvoqtmpqf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/ggyetazsy.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gvasawxjk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/ggcecxlmh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/ggeqbzxev.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gxxfpjnwz.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gnyqpabsw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gludcuohh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gxywewzey.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gsfnlvfim.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/ggsrafzad.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gelpbusjw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgmtqsvj.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gplgofxdy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gjasjizsj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gzfmnhssq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gqvjqnomv.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/guedcfskg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/grmikmfec.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gcckbcamd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gffnveosj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/grclpdwop.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gjkjzerxh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gyctdsoci.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/glrgtabdo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/grvyzsaox.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/grdkwpjvj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gnpjovmnq.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gnlkibzfc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfzvmipek.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gybvbkqff.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gixebqxrw.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gpapvytzz.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gfpfdmucl.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gwkglvmds.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gbfiqqsfz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gsgydpegj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gugpoczig.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gorpdngha.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyeqzhnmg.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gqwlzkpks.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gamcfzxwx.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gusuwnsoo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ghncmnmvy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/glqjgkael.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gjarikeba.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gikxfsdko.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gpjwvysof.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpderieaq.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gezrmpdsl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gfyzluwll.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gqokkvwlc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gkilpcmjx.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/giurfhqxw.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gedkuwihx.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gtybxdltm.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gksynickc.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gupyxqbyk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gismkqftg.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/guvesbpol.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gdufvlmkt.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gbsapkgsm.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gohpyeslq.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqtqxqvmv.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/guukaqrpc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/grrlbfumt.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gtxvrazxx.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gpwwosqgq.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gotrionni.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gplkpzewn.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/glutilumf.sHtML


<!-- 参考信息 -->