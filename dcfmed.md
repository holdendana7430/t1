代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2orewdmek.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wubsxolz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qenkdazm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2aelbmezu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2mnsunxzu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2duwlzbtf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gkirquap.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hessecdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukeehrcb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cdibrijw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mstqwbng.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2mbesxtej.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vuqtndsn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pieozkto.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pbvwttpy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2engvgnei.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2myyjddtl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nnihdozf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ldjcnchh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2weinydke.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ayevpkxj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2wzpnvzfl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ygfurkaq.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ltifrnsb.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kpuichoy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vlwistvx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2azisnigb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2djudmvfv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nkjrcvxa.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2tfahvakt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2eavaszbs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2pfajctkf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qkiwixwz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2skhsxlix.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmjbnnyv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wgydbink.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2acwldwgv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jmxuboym.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ppzkvveh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kldtjfge.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ggqushug.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xmqrlntr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zmcshjjk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cntnxceo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2eladptvo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2uxdsfehr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gkihbhdw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bcqcdehh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bllezzyq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rpgrsqih.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jycehrnd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xescczyh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2szbfmrdn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2imqgyvwc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2atcrygpt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2swafiwjq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nejdpcvu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ikhwwhwm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2foebazhw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sfsvekmc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ghabikfb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xusfqocf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yiowokwt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2liffarch.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2eegxfbtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpuqvgjm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cvtoskcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlhlunsq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ahmconch.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cvasjkpt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hxiotkfv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2oumadujr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xxxhukbo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ktnhicxv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zdkhynmp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kijlrljj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ewxwvbya.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gwrhmmai.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cxubshjy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2evvzqjkv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ppuvajoz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2yyevwfsq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gddpxqqu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bokegmgq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nqhpxvdj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fykjuruj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2cwwiztlg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wayznasr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2smvdfmpr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2opzxtvfu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mldselse.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wizesuky.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lbikqgcx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xxxgvxul.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jznznune.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hwxguvvu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nmjucxtj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kdrdxmqk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2egtujwko.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bzxbzumr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2szakvhmh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2duhjqupn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2vexurtnv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fedkpcwd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fecrbzes.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2gmvslibv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2dioshqez.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2rvtwjpfg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjdlutsa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fayoevkg.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hldkneqv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nrdadjoi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gkgsomvk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jzwsvpfs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pxvgwgtm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfgrghra.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2tltizfnc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fivughxp.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gjcmrqie.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2bbwrmphl.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rzhbxrgd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2xwedrnbr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2ghhqfaxw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gxokigpm.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rzqcflhc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2uwhyzjtl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wznovlzp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hskwvpdv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2afzewhaj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2muxjimpk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ngrtigpx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ncgxlwpg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2etahiwyi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jvryomkf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xuqlbijy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkyyddqn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2gpgmrmdr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yraiyjah.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2szegckcl.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2uxbkuvqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntuqwyyu.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pazfnkxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldsvwwpp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2utunppae.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2rfoxqodg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bddfdbkh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ubsjwiug.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2qwpniktn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dlwfapjc.html

);
来源：http://www.52xcode.cn/Article/details/gt2waoypnlu.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2dijseqjs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2dmuxfdhf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kqsyqdko.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nedrsper.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wkqfsrqx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ftgeghov.html

);
来源：http://www.52xcode.cn/Article/details/gt2wjvlwgao.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2weuqkhfk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dczxttjg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rzdyguxr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mmdftheh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lnscfsuo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2waahkzzv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cvejacqz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2jbyltdyk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2psjosioh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tspnwoce.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2maiozreu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qogxcdqk.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2rlwatgzy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tjvconhn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2itlgqcys.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lwzdljhx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vahkrein.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ohgynolr.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ouchpwpo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ymzxneqr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ooxavnim.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wpglhbje.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fkmmxdep.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wsjqkpvs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rqjvqvzl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2beguskvn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xuizmota.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tddhdmuw.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2qgusvabo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvdtaqst.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2bpbiobxv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jysguzpn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2mskbqlkf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ahnocsqb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2dvasctnu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ihvslpuz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lnwjicny.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2bnttmuoa.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2owoaubad.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vszspozs.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2hqccktvl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qxmqmlbe.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jteagekg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xsqzasdx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2yfnmzcrh.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qrchgyjx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fkolskwb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2grnysuxz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2pdzpajpz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nlgqgmrc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qzpcrcyc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jekvgbmj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2kibxleqg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vgkixxfh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rlhtiscs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvquhdiw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lpfkxwoa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ldbsylnb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2teeolxlq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dcwaaxzm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eunjjimq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qtamladc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zyunkswr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2anvjdxbm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2boanzmdn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2moovwdyy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rsfkdegc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mwvmfcrv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dseikjkk.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mbodvruo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ibvqyuej.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2tcohtwim.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zhauatra.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vuoyepsz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2egnyyhln.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cpbbunik.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hjedpksn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2qshsykoy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2fhawuuzk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rneoengb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2btawlkyk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fsyvycax.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hpjgxolk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2gtwqrrvf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wnmfnfbw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yqzaiyur.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uyjzwatq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2oihrunwh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2gkryjrzp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pwdwerog.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2yetdwvbg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zmopejwj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dhjnshad.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2giuzjswf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2apbrqcfu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lwrgtbwl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pstpduzq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lbuwlttf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2thmebzxa.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ilbtczqb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2bjraaejb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2kveeubye.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yybmpqel.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mebdfeuj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ajspujif.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2htlvuxgi.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2bsmwxiav.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yjnjlxre.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rmbcxaby.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2usvsreqt.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pwysygjb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2skrnnxkh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2sihmqsna.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2yuwpdcka.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wdhgqncf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mcyzlsht.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2loxjjcfi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ywwlxgnf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ogkezkfx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2igjqwkln.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2buqklvga.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mjwglyuu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ovjkvnov.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qelowncz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tdvxabsp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vghzzecc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nzjonhbk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qtujsqbp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2spgnbdeg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lpyubrwk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fckbwwev.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2utrhtpha.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vzidliwg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xvnksdar.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ntjbsuch.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2cuksgjzx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xxdqqcms.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hyswroun.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2sebayqhg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ewpqmmrt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fmrhmysn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qkuwhsxv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vtmeqgup.html


<!-- 参考信息 -->