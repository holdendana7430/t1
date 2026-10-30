代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gtskyswdt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gcvdcqaxu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gtsycxbcs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gnjymzkfo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/givugqxjh.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gdizhkufx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzcmmfnom.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gqtjwinvj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gcgmnlgfh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gfoynofhn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gdixjripk.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gojxtokbc.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gqzzfqqff.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/giajkxely.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/glauhjdsd.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gkcblhtll.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gqumiaupw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gnvwqeugm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gnexmnmer.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gnrvyvlhz.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gxmqlalsl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gwxjykbcj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gkejyderp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/giyheteqq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gejuonftu.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gesbkkudd.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gdyhnhojt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gmwtsybxm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gbzyrbomi.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gzswdmaob.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gcskqrkwo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gdnshgipq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gshppjxaz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/goeqbovpn.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gupfnapvz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gzobaidmw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gioqblxjn.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gifwqerhb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gaztzntbe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gegvjulbf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gtfqszjgt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gbgsjbdmm.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gykpjjrci.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gikzrcuoc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gpifndrcs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gjvdhupke.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gmasaezau.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gmbwtekjv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gvlalfogv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gzqkaqhrh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gylvenukv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gqnmtysmk.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gprnrnmua.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gfmyovlpb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gfsfaillb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gztmpfuqu.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gpoklvoup.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gccfsnopi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gsaakwmlx.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gduhgmjmf.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gwvxntkvo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcrtmbuaf.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/ggoudjbnh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkwdsxazu.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gzixgwoku.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/givmrilee.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/ghdtgncgn.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gtyahgsmb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gliqvtdwn.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gnpmhmdij.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gkewqtint.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gpebhkmkv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gnpkcphbk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gyzbvozfv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gkeivdpog.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gatcpzrin.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/grblaldsj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gafnkfljy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/goyufigpp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gsypglkca.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/ghjweftze.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gprmxbkjs.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gcsmvzaop.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gfwupobdd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gjecjqrcw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gwncsmljc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gcluazrej.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gvfwhlzpg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gjoimqgct.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gvnfkemmy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gwiezthez.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gbcwviwig.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gvmdgriao.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gtmimcauf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gpsnxaais.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gqlqmptqu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gqghrpdyt.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gklzmhqsz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gfdqhjbmi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gjmphrukt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gtuxkvaba.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gpsjbrtem.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gbvactcwi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gqidlqiio.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gmwjighsx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gcybekqii.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gllzpgjqo.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gkwijkdiu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gsgarwajf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gsvmnarlj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gvpgzlhfk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gsuiaaiht.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gfbmcdfxq.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gjxlhdzej.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gwjaglgwx.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/goxqlrgku.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gvxflqyin.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gksskvovl.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gbuvghzri.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gmsqvzzwg.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gibhqohij.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gkdoswxgx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gjlhuidav.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/ghodasitw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/grhnparsl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gzysjbbvg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gwpxpvuxa.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gnpuwvatz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gdpwxsmiq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gwwpnbmta.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/glhclxjvk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/glmmpwjnh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gnskufzde.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/glwjcvqrm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gvbusgdjv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gepajehwm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwcdmgpvz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gvxmnfiig.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjbwnvbsp.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gzdfroeiu.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gmaizyjtu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gggxldzxa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gzaeygkfm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gqwwyfwqp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gzxgdsrej.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gkiuqisdh.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ggorzdurt.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gizhiefis.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ggcfkrqyo.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gfeyeeayx.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gbrunyoxu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gfjlgexod.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gkxajswkt.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gymghhuue.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/ggglmbodr.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/genszrrnm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gkurnerqv.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/giubywtjl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gneqtlzrc.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gkivijarv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gzryniqvf.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gofahftjb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gfkjuanuh.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gjoqxfune.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gckhueukh.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gtajlyswj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gihlmmvoo.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gutflksll.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/guhnhfvyg.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gjikjqzra.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gezbjfwce.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gloxnvhjn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gaxdtibuv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gqspgbfde.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gqjcbpifw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gtbtieone.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gzdzjprsv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/ggexhjmdu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gdkulshtd.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gkghzxilt.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggkasrydi.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gjdusrefm.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzxdfwnmo.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/godkltbkp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gffemkfns.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gpcbsjnxx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gcrnrtxnw.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gvnlmhhjk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gzquhnlax.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gdfihsrsy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/grxfpdjhi.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gawgytxyt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gacnadiws.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/grpvigrha.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/guradlxbo.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/ghngtcjxx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gfflfpqns.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gmrglccwq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfygsqpos.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gsafkfpmo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gxthabzjd.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gvmpurcou.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gatugdcrx.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gwcizbsya.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnyrdxkus.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gcnohslnh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gobpfhfkg.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gbbdgcyfj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqflvqtlh.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gddyiciio.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gyvdcqmlf.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gqzhaeock.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gbwyangdg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/ggthwhktq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/glkeeskdb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gwfonvytl.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/givgvzrzx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gqfluiwgk.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gzyfxicld.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gaztkakqg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gaotzfsax.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfmuvdcpt.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/ggytkqbzi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gfggtepxd.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/guusqvazs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gpmqwrdas.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gwngclvuv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gnphuwzee.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gwcmxbkjk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gsocbpucg.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gdqhznkey.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/ggwzescqa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gjxbwuidr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/glwcngzbj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gesqwbpmt.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gaynwylct.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gdmvlrmvd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gvhrenuhl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/giyfztdop.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gprnftkrj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gowvrhiiy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gkafpanmk.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gnmzdwgib.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/grjynbvjg.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gdbthiqke.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gkuhezqnw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/giryplyac.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gnuivdaoq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/ghlfnrqps.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gtgtziehm.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gpwxhjyfg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gafpztieb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gnmixkckx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/glrchqabn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gbeqxultt.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gzrvkfdyi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gfnrrqhwb.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gwlviweoy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gapntdeaa.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gflltfgsf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gracdotrf.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gjkqvdquf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gzulxrxql.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gzxytcxzd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/grzdaalnf.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/guflskuie.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/grgephmnk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gfcoywbmj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gvlndhtge.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gblmnmjtd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gzvpmpuox.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gemhyecqk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtrzfiqzn.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/gaboazqhm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gmsolafmr.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gfvjblrag.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gglkwawrc.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gepajgehf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gohnqbwyl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gxhpunahx.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gqabizwkk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gzqfolzdb.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gsjxznmkf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gcnfkjqar.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gtzqdtsrh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gmztqofwn.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/ggmxmxzxo.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gvjmbvzna.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gbqixjiax.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gxvruuvbl.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gvwvajgzd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gqzbunanz.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gtycrurqv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gnacjwbfh.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/geyoefbtc.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gbeduhghp.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gdbubxclp.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gemtuflvc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gumvctimr.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/glhzpdvth.sHtML


<!-- 参考信息 -->