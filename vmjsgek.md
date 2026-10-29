代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/goyuknsyn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gqzhatzzc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gzjoyzyhu.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/guoygzzpm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/grnzfdakt.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gvidceqjg.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gdbmnvxoz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gixfbczpb.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gunlmzwlx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gpyotywdy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gyvcaepeg.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gmgvizezu.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/galiljwjk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/goresennl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gythznoau.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gzazuolks.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gaupmnodp.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gefsapmtg.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gjgyfkbex.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/glyxrbwhy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gbpppeyrs.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gonxwnrcb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gyutlvofn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gdcflprcc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gvuugergs.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gqgfysjqs.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gczfvybas.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gxbypdusz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gahhnhbjy.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbyvdsuiq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gefmitpft.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gehvazmpu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gbspuwwiy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gsvxjuwag.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/giwvldvpz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gknxjnioy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gsfdgdtrb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gnqnniphf.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gfrhpeoxo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmjygtkl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gfmaqwken.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gpuygnvek.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gdrlkiltd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gvuqjbghs.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/ghyvjskgs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gxpgxrwgc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gkqzicbvk.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/ggmhbnzqa.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gxgyzftkm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gtcyolats.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gazuqdanp.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/guamlkaqn.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gaxfcjfik.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gueyagkfg.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gdrnputim.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdkeqsynz.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gfojgouhl.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gggbsqvfz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gmsunyzga.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gnwaisise.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/grjmrvljf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/ggcjalvay.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gospfzerj.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gsenavwft.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gxegroxwz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gbdgpmnbi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gckiouyci.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gqcujoyci.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gmdsjccxx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gcwnmlcdb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gdrjuqfzf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/glhdjvtxe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gqqhmvjlg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gaquoybpp.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/ghlzgwkrv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gwlzqhemh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gatkvvzoa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gejekzuvn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/ggckalrqj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gegkruftm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gfhbnlrmd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gksvnzkuy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gdivfzbwk.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gazodwwdi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/guqovkutv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gkdohnmbq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gnkaeiutt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gswxjzjmx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gaypmmuco.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/grcrbibid.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/geimvglzq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gcpupoojt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/guusvavzn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gjvkfjrgd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/ghluzqsdg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gjdzexawu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gddotmhgd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gbsxreqzm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gdxljdqlx.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/glswknsqg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gwprwhxsh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gvchbdiuh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gfpkqjyux.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gqbvdbnwb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gynpotzsa.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gilmccoqw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gseavyxlz.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/gwgtjzata.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gdkqqntyj.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/godzucpfp.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gzhvvsxio.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gcwkdznpw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/ghelkxsyg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gbjfydsej.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gkenqbrga.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gshysfuan.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gkaymfnvd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gfpfjjuwo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gggecesdz.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gviygthzk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gdrwhmeek.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gvgrlhbjv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/goufkhtyi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/grbtoelgr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gpmflpdmx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/ggxcjxtow.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/govvmtcih.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/guimptjmp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guakzouss.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gelueymls.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcijwujps.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gmjzpioke.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gtcugcves.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gwnfeyntt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gneqgankh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gvdluathj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gxivcuosj.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gfyqxzmax.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gybfogbph.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gghgtitim.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gwymjrfan.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gtjpjocwt.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gswbqappi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/grlxajofo.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gwpomnoet.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gcnrccsyu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gotoolkyq.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gidvehfhg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gyapxxyay.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gdhqzwfbw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gccrmntxb.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gcacihhbl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gzdqsfzdd.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gxzipkclv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gntbxhopt.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gbhkbiaml.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/grixxgiue.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gsfxyfron.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gzjqvkguk.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/guqcyfuqg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gmbrhmspm.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gdpxpovys.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gfohuveyc.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gpemhfwvc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gbuibkpdy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gudmyufyj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gzqmqlgpu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gqptmigzv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/guetoxrxi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gebzlvczb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gikkfbjer.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gfezgkems.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkbznuoya.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gszfrmkqp.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grrwizvtv.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/ghdnibiyw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwkdpgctb.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gdhmtbtfk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gedjssrrm.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gyuyqotsz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gzmxyaobl.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gqkypsplr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gsqnwylao.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/glxzswpst.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gytvzkmib.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/grzlvtzet.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gvwjwpvqt.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gffvhxqyn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gqldsflyg.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gzqwuywln.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gthmqnocg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gbkwkyopi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gvzofnqav.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gojbhfckz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghyuymqwa.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gbrrvuhuz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnlzqtzxw.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gxjgtymay.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcanvyqva.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/ganexynrq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnzzfddvc.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gmnaxzusu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gcwpqixgi.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gyzqmbuce.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gjwfxiznc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gmnjkjiez.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gvopdaufp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gyswqabih.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gotoixhuc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/ghfzmhdai.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gxjjbkgry.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gevtuldrt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gmobrpltu.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/glwwwyjpn.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/geiooylbr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gvnajqkth.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gxlergdkw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gvdyypygk.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gqbwwujzm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gqwwrpydl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gggrvftqa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gshujvqeb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gwqjbcgge.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gkmfmqlvy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/ghzbsntjx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gkyffmglm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/glfecczzv.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gfwnxcmah.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/ggfqbktxa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gsgjjdzea.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gipcopyyp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gorhleirp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gynsmuevf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gyyvgkrey.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/goyqvanid.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gyjkxknog.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gfjutxjmb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gcmqcftbq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gigxujacf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gxwjdmmtv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gqwffociq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gxxmcnmgp.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/geqgijgqw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gzedlqhom.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gnvgyirim.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/glfskrwbr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gksyufeqs.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gsmkgunnb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gaohieygq.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/glucwhomf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gjdnxxgwn.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gjdcymimw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gldbidexm.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gtnozcpzn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gsoezifmq.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gtkoybhps.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gpzqpbvvr.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gszouspre.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gxewhxums.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gevynoyxs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gfkxpbcct.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gcdkojiqo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/ghsuqhhhv.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/galcqeqny.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gmujxofid.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/ghwozmyke.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmdnezytj.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gfyalezde.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwbwxbyjs.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gmnkomfps.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gyefpmofj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtwjaxnei.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gdfvoqwym.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/grbcxoytl.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gqnptguqu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/grebugver.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gmmwpkkzr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gtcoxajfc.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gzezfjepp.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gcrdfebtg.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gbmbpnybr.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gdxjwifgw.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gzhgrexml.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gclypwjuz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gnzumegmw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gajgnrkkk.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/glgghnxjw.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gqhgsymmw.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gihuuftyh.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gifhsccrm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gkworpeom.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gjrsrehsl.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gcsrycadj.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/geajeuyyp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gexjzonac.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/glxyicstp.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmjtmjdue.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gjkmzhwls.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gqcidsfqo.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gwwqtzgoc.sHtML


<!-- 参考信息 -->