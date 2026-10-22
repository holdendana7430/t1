代发 wailian999

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2aqbqjdym.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lkdcsisn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2bgfiansp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ngjarhqx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kpqchafr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qlcwaujh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2rdwtrlrt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ssndarij.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qckltvwe.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2nblsmhjg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qbjdyfrt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2mykfhcuv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qvyzuvml.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dnhiosun.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zzrkpuxu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2cakolhlk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhbyyeh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqeoavk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qjqskzxt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2njzbgmxb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ogibbjtb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwfzsmdh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vggbgdmw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2eicliogy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2loymvlqp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vpkpnpsc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2npizdxjm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jfjackpe.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uwbxrfxx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2gdyufpwo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2weusewbi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kgfabops.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nhaidmcy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2aetrqpyu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2btvxqepb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bblbzccu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ugsdxpei.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hndnwcfn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lnrkyplu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xvvnnmzu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ixrmnfdj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pqyyupqk.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2nkkmkiqo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2auskzxjg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nxnqfuex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfqwwmeb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dqvkkais.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npvhlyhx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2seomnjsd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2bcrkpowf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2myrrgpow.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2snegapvb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lsgnvqtw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rzmegwvu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ubbrcbco.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2yorwxljg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cekqrspr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2merrujql.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xdrdxgcq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhinjxbs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vzmzpsqf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ijzmwyzd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ngvvorch.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2zyyrqquf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmbladur.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2twdvbxie.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mbsyitqi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ipkugldq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hgygvnhm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pxgqijqc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2updeurgs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2wvahwlpc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2znzczyny.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ktpspbpj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2yxingccq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2xtjsxauv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ulxruixa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dkjpeymu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sdooiofv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fhxhozci.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gjqapijk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ukfaymsi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ngvffkue.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2epeldiiz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2dqyazzez.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2aroyjtqq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2lqqcihuu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wochhgpx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tvfcjbmx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fzalodsv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uhpbbixj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2vthdbjix.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gynyrmob.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ntplupci.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ncqxodbu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pgzzjdhr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ardqcvyw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2bhgroliq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnmdqzeq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgrbghrp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rhslliut.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwqukdzl.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rvklabcz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2dhykwzov.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ozxtuclq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2enveaiwt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ntyepkpw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwxwlovv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zchdyacd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bnzonoci.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zwepsyyy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lmjpzvva.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zsuzidjr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gobwnele.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2mrvzvfno.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ltqgdsdf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2rsdqxghe.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2mdeakxmj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2abkovcwd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2yrvyxpeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glkmxqyc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2raeaasbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnaghdpa.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2eyylsmpf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ycwdnhyj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2klzwbocy.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ktuzdaax.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rduzzsux.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2piyckrdk.html

);
来源：http://www.52xcode.cn/Article/details/gt2drlewjnq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fxoqtucb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2ihjxzjgq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bwsyliwa.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hqjuqpli.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2uxhnehos.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ytiqdxri.html

);
来源：http://www.52xcode.cn/Article/details/gt2lfonycdk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xmsplueb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qqkdikfi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2badlqbdf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jtmabvkx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2liczljvb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2rkwhapei.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wembkvez.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2yshxpook.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2gdyntgle.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2bjzukhxz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2mfzfmdmi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bmzqnlfu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kzmiwrdo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kcebthmd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gdmljiba.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2chkvszlo.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2ctideawe.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2jjfpuptb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2qudkwovm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2mlqchqri.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wldafqzo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ujmktszk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tnuhyzrb.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2irikohhb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hvlrubwx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2uaqmuxrt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2llbyprat.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sgfmalbx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2wneayjtz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2chgndarz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2bqlxtzgu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2damakfyl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hihjkqae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2kjscwkgx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2wqerizgc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2cspbydvr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vzsqupkg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ehckocsk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2vbutibir.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qjaviwve.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2gasyogqw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wbrhjbyt.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2perseiuk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ifzxsown.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2kwvzjcye.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uixiwgaq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zeypxisb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pegwhfzs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vafnxvdx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kzqezpht.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2dkpqkxjw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xpaavrvy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2yyhzjeby.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xerfhjqj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wizdqwzn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pvirmmdh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dbjazokf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vppmkarf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2fqzbzxtf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rpenycst.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mzzbfhnd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2spexkepz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rhopkttu.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rfiplmjq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hiifoyxw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ukimzgrf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hrkasmcz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2pctjxoon.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zctdkfva.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2grsrwgzy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uncktzet.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mxettmij.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2haxaxckp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gzntyqur.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rumpdfxw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2afhhuxsn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pahochfr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tgnrndkl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pqupobmu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hhztxrwc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ciiovssu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kujqhjfp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xcnpwsss.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2lcbfrxdd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wjuxeknk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nkfuwyak.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2cctqzhzj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dohwioyc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2pklxctjj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mmvayaln.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ybgugyfy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bzehzldi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2cadcjfzs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2zzjjygwr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yqrudybg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2cnivkess.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vnokzktp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2kjscofqt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zxwvjdzp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2abhcoeyr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fryolmoi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qfqlqomm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2psolkwso.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tkvwxdig.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rcyjlutd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tkooifmh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zdtnxcqr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mnyacjlv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bttarxun.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mrsahoui.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2puhhvxrl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2sioxfymf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2efsaxnos.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lrqobtye.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vlsingek.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aqvesiqz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jnqrpubr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vxjfmqyf.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2jmbvfiyy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2inxhpyhr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2znbtslrr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uugakotj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2yiurnhlt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2blqotvds.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2lgxlzycz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2oufxzkhv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hrwdrbxw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gknbinbq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2haqvumnn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2szjyoihj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2suekrpdb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2dssracsv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2moxpabla.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xzshuqds.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dasptxjz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2sbsacuob.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ezjmlvmt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2satskyny.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2kizaflgu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2birsmhht.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vymjozin.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wxfxfyve.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gtlhcwqa.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hxzxfkpk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rxmijoso.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2sylicrao.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2oykkspyy.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fowufsck.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nkqyslhb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wbqxfwdq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2mgckpllb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2alcrpquk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2krahuzse.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2hautcveb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qnnnewtd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2delupmwu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pkcidrwm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sbxlcysd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fqvtfskn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ntighczf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ktpzljlv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ybynkxyt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2erhqhtbh.html


<!-- 参考信息 -->