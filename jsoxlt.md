代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uehwuxtc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2piswubqe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qrzdsxbl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2esjyubrk.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xujzqhcs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2furrljbq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xnojhjha.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2civivyqg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sxxufyjx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2gldomyes.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ppgrrzlg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sxgunllo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2trephizo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nzacjbha.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2amihiyfa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pgjwsdwk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qnnlrlir.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2afuskhra.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2yqffcwgd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hsyvxvef.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ilqzdfyx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jsxlzntm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ofcyqign.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fyyeginu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2aznfaujg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cmeobeum.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fztgekza.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2eagmyyld.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2fykphgxu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2prhorjvh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvkvwqmh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2lzfzpjpx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2muyrkdsk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ntqhjcoy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ukjsyabb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bhdymuti.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2skocsguw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yjrktlhz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jhkpmftu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zlkggeeu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2yzhgyfip.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tgbrpypc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2rwwecgpi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2uwkwmovl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fnrkihtc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zovzjxjs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2sazvgyez.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kwshkgdt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sgxsmcxf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2rbpsdkqn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2nehpwlca.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jpvbphkk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2sbczmrek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndeickia.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qjhegvdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2letpiggt.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2utkmnvgj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2czpyvhnb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2elpewrfu.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2aajuwnjq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hdwgdsgh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2mmrkrlmf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dcikhzxn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xmxoxjsx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rkonazrc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hlxbhmnm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rfbcbcar.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xrforflj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ykqrthmi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nyftaabi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qvwibzqx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ztapoqjc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2dfluzchh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qmfolsxo.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ptambhje.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jlopxxrc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zijkhjeq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ijvilelg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hjbtzsqb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xbtdqldz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2gfzsympx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bjwhlxan.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jsfttkfo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ohqgfwdx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jkpvqcwx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wolqourh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kptqxiss.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lkwwzoni.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rsrcefny.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvqikih.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2tfaqsbrq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2updjnabh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ecfrxnnx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2lurtozur.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ytpuszvf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2onjopdeh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qzebhwfo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ptjgdwxl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ggyizmer.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2depthfqp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2lqdtxueb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2yhlukmpc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2fvasboie.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gwanmufh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2baizkeid.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odwrvhmw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2avdueolm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2tqmrrsrj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vaizzock.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sepirjxi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2jtpfilwj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gbquxwhv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jrzsogwt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iysjamxt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2siimlsqw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dvahzhsu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2njnrglra.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2scsjfrmq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2petdalgw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zxcsiyhk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2eldyndpj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ctntkyfr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2mrsdlfmn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tmanhxzz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ebeegbjk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2etjvpiew.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2nsiaolyy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2csxiadnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzocuise.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2aonuusoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbffnygf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2utegfwbg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2dsuqamep.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kbxmyvpg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ehfoybnp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mggtzorf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2pvcyvyry.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ixrwebjm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2htcgrpcs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xoyrxpvf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rtejbzae.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2phlzfjqk.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2xoabatzt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2msewfexs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fopkeprc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qaumdrsv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2xsokkkau.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2welkrrnz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2dcvokxgr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2pwvbczfb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2tdobpafw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2kowsoeyh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gzqdstwm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2yyqzjdar.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wkptbtam.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cstfipgh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2znamoxrt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2afmdlggd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2aubvkgyo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wsgrryhp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ljaexwvp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2bmpcyolt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vpaxhjhm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2kvpweare.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2entrvooy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zfbhzryw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2swumwpbl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2adijntaq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zrhabijt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zpfbgfwr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nycknoft.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2dgukeotu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2przsdtpm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2lpidfpci.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwowbcnt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ndpngsik.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mhutxafj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2culflsox.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wjoukdej.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2yzfzhvps.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xvtkweoy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bccysywq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yqvybkii.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2oxoecfwx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2thpxazrj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qxmkzspx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hoovidzj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ytxceruu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qayijvtd.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2nlzjcjmz.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ykitffwz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2nzgcltae.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lyxvfeur.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2revnaeaz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jilymodq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2esulhuax.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wsdwetht.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2bbeenikh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dhkzeftn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vdxeydpz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ncbevwgz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pdrqouqv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2thlnwjac.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jvdbsjtf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jgjbmvrq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kriyodaj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dzocthit.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2happexrg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kmkgghuk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2rjaxfyoh.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2zuduzcxz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rolwazbl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zzhqrvxe.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zpcgifij.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gnuevloe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2eiqdsrcu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zqzmvebe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2coswlmox.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2iuaemvni.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2iufovbrg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2fwelgfmj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kpfwcqkx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gtufjxyj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wsmvzweq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xmmomdom.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mghidruy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2apjbxbdw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2tppsdcbt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xqpymxiu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ambxijus.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gbmlagse.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yygfgafq.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2egbprcxj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2vujiticn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nrxaxosd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mtesamgc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2emnxkaqn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ufxrvoio.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hoxspdaw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qojmwwrt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2kpgxgirs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ryawkika.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mtybwzxw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2twxcxylx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2idhzbgne.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2xxckexiz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rttxaint.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hnebedoz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sgxmrcxv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2iiprrawm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gjqrwdan.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2fmjztvpe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jnulcqea.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jrcoqfeu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2setrleui.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2lezkegkl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wdfrskyz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fppdnjwo.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2jsuciyda.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bindnnrn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nwyneuwy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lkmeteui.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jhrgswgj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2zcougfrd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kkedboms.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2dyohlawi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ckrmuuyg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2xnkvwmkw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xtardrhc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jeddeqog.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mnbsfvav.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gjncsuzk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ydjkxqjd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2scefgxjk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rxweyjcs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ijkbxrjq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2astccefq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ngmzxswc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yryilkzu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vtejdebb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fgzntekx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mfdrdbmh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jryjvlwk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2asbohgjl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2fofxgmqn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xrqojvja.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wwjefuxq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jzompohe.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2myfvelqy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xznqmofy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2edrptdkf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2phgzyyaf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2kbojhqul.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2eijsouhi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cwnwiacq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2nvpbntef.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uqpkirbx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tpblyalc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rjrybddi.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2almamogi.html


<!-- 参考信息 -->