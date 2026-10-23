代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ppeclqnt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qtwekmkm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3olumnwxt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ljdhqhvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mycyntgq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3svznppzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afighsih.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lxelcftv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ybrdrgby.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qqthwgap.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mqchqlxv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mkssjaea.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3tebajhjv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wmvmwzlp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3srodbdfw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3futefifz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dkjmxozu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fchvaohs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ezbccbqf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3scgojitp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3fyvsqwrz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3cmmhcygh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3rrtulvup.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3bgzflzjj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rngaijnv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wblwcvag.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lqsgxgro.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3jfbmxbyk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3chtmhlar.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ujcrwyjn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jbwmcfuy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tjvkrqqc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xowpqrhy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuuufdyd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qsyunxnx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xttonskw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ndoyxqbd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3snajfxlg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3upqbjziy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3raaqporz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ssxhggpi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3yryyifcg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvbioiwm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gnbzwfvu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dwkzbfap.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ikmpqdkp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3azgggdfj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uoainavq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rrtmxhwy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3gzpmrwos.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bcxqqaym.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwlraqen.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wrtupsli.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3iqsgjxun.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bckjarib.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3flmvnsjc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pudncouz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gmdppcka.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bwucoemp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ttanrwix.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vpsbrgmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljiabzdg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3anfgezcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzxspppm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3aibpmvrj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3sfodmycq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3kmkbyery.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3upwzrltu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ekjqhjzx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wpdilukj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jdrfacza.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nubvdyqi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tftbhmva.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nzaxctuk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ladftgdr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3owfjbnds.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kpunuqmf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3jsffqewk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jizaxmqv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3hqyerugu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itrmhdty.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qxpwzdlr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zqowmebu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jllhklmn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tpievosz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vcycreel.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rwlsniec.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rehwepxu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lbgoiwbl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3gljwtssg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ccckerfp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3anzmmujx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3swubkwao.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3htcunozo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ldwusbyv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lpvxdcen.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gyvddasy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3igwctsma.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vkbjpcbg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ecyszkzw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cudgkujw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xubdaqpt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3trhtwxke.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ghuhqpca.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nuqpitug.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3llvlqgmh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fobtpvnh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3skoiqeel.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qdrbatjy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3udcptukl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3gznlvgev.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ngomfuvf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kylqdzzp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwrtdlja.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xknjquzv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rumdcqxp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cfnfmtfk.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktsyehhi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3gbjykfcy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ppiwtfbe.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3rjnslync.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ezyihuxw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wuhsokre.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3cnonkowy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mhxbbpmt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lkemmdxy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3imjiecpu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3mvecelyh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3csxjilgv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gpirpneg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3jeeafnnk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtjvmqac.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rbjxeomp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3aszuzcku.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ivgxtabn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3zzzvlkxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbcxegtl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nrvfyxcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3volqmvpg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ijfgkrii.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3tkqkctci.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ppkdqkpr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vobsoyjy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3eglrgahr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3khquepek.html

);
来源：http://www.52xcode.cn/Article/details/gt3sanfzzfw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3nnmfesey.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3lghyrpot.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wwrdwyqx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3feqjpekm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3pksnesdo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zlsxuofd.html

);
来源：http://www.52xcode.cn/Article/details/gt3tsizvxuk.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3eesepvnr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3avtftyhy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3yjufcgmf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3elnwsacb.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3hiounqqc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3okewyfuh.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3urqolxbl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3bndxrthl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ubpuqcjm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ftxqaetc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3oqujakir.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mqjhbeda.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3cpjynwbe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tlabeohl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vzonlylv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zodqlmqk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ndafybny.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rwahzytk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3dhwtvxdk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3iwcvxwur.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rxqzhbye.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xupzdbvr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lbshionw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3dvthopic.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yuovwvfl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3aghwdlww.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3xzhzrmbh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sqttwfbd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3doqunhkw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kfjxfdit.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3rjulzzid.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ninshjww.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3omqurtco.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ckplkcfm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xgqxcqzh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3qpbxiggw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3sbypfdiz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3itfyhhjn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3utmhoifm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3bnwkfygc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3sekinrib.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3uxuskusp.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3xhncrszo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ljdunfpq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3terngrzq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zykfflmj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zwxvbqnw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kaedggzv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3njoxkows.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ypgiobjc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3nwgvnphs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwliiwaz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3tmcruayf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dladpdoa.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wckooyrx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3audmjyiw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3dzmevhuw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3omkfnxfe.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xqmbcbxd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uiugzfbc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nqpieqyg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wbtujzvy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3udpyycnw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3rikemczw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3asxljwcg.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vuggqdoa.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bdswadsg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fbnhurxq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3knbrxjhg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vpgkanlm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ixzcefmr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vxsfvxzr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ckxsqqxc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xjxomeje.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3dngxyhut.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3hlnufizs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3knvcndgh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3lvbpywsg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3sdfbdgud.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3flvodrel.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3enlvhkwv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bhsklbty.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cozbxwmn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3nnlcrihx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3clxgxgvw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3quyeevfa.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qlqidcxt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3vdrxzerw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3lotqzlyi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kutqytba.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gyoqwekg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3uyfkauqt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3wvcjohzu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3fpgeocqo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vjcgjpex.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qguhnylw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hobdapaa.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kklvtbxe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3vkulhxie.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uzapbice.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3linppdcc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3trmrowaw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3dwmgomww.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3aptwcywl.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3vwmqjndu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uomfiqyy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xtkaykzd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3garcxuqp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3duigourg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ulpwbkpg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3njafvnvc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3syyjbdld.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3gtibkqvv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dfyfqncg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ifzcidor.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tbvkeler.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3whyhozci.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xxnaznju.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pubxzmty.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3abllpsjc.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ziyhdjpq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fgnqanam.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xjtprgsx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nuwywvqn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3svnvinwe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xcoxhwpb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nfsjobzy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3dlcyedgd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pmfmqhgf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3xzxampob.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uuogzoaj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3kqelbqgx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3rjxikail.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qgwnvqxp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3tiwcxegg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3oaogdzwh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3hagzhwqa.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3myhaquwe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pglvqmnp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hbvjhztf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vkkmsaga.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3bdnozvfs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3skkngnaz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pllidcop.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qhxglmce.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3llssuyuj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pakeyqqv.html


<!-- 参考信息 -->