代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2paaqbnwt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ykvhdpcw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2luatdmxt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ehpbushi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rldeyuoq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qsurknds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgwqhouw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2jmbzdmzd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2onzofzta.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qttzdqtr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ctnuetqp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2seezmzus.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ynyvfzxf.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2kbuairfx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mizytcus.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2snhrwohc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fuksdldu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2uykuamts.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2pidhsnky.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oxyjqlhs.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hhhifmrv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jaketzxw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ragzkhbn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2vybtjiov.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wttapsnn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dwugldwg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zpekgvmg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jabilnql.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2xdeymjja.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sgkfanmf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jbnivdcs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dnyyapan.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2uqbriiku.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlvkrxoj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xwkhzwyo.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kjgdapkc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pbeszxgu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lyqqnkvx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2agyhxssc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2yzjwkpwi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rzyjlmgj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2szzkckga.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zghtrrrl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2cktuposn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kuucmnhp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zortklqj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nruhuzsu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fuufcwxa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2aomxyyzx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bkdyefkw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cwzxivrh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsoceobh.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dwlpkfba.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2dpoaqved.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jyarxxyv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qjacqoki.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xwarxgwl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wezbneer.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2eafflnjn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ntuhvvlt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wrkkwkod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikzvoitn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2iosxoolp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnqmllhl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cotqfkag.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2eiknntzo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2fvmlsyih.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2blzerqqf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yiimoxtb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2csmdxekk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ilncmwai.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ejwywdka.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lpchmucf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gwshlsll.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lceavvpu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jbdpamzm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mwrmexdu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jkexmuyu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fbdorkbc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2poktviid.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhtojfyb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2fxlyfzfz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2maedaadm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jerflngr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2huwkrnkn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2botrexdt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pflnsxlx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yakiswrh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2zzxkvtrz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2dglnvkeg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2bdodykpj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2obngvcby.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nxodwoiu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cuwooqaq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2odkagvna.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2khxdznmr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2djtdbjkl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2jequtwra.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2utjhsfmx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nzkmjspu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hjihnbdt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qzgnymhr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2biskqyii.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2upcvxaib.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vluazumb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2nzxcngqo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fmliaymx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vrcathgm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2tfzvmbym.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2occhwyyy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2znmsaxky.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bxcytjra.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vkvmxnzs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irocufoy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybrernkv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoduygvq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2guehqyfj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nzvhddey.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2bvsvygkn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2houzonwv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jjtlrfpv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xvowwdtz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfbkhtav.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2zsbiubhx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vogmjrzj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2gbanmhvu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2galnbcqp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2asrdiuaz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jcoubicj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oelttkcn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2sshcsigz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2suyxquoh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2dcsyhsyy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2xqoaxejl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2kmjvqnmz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2bhkzgloa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twuztglb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2usemlsgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcictszi.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2djjrzwzi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2eevposev.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qmzyhpfd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2drbqfemn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2btkjuwnt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ttblmopz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zxocayxx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2avocquwe.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2lylqxguh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tpdogmnx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yurmbnxp.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qgjwgplx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zluasdyb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2purypdif.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2tuzlymel.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2aiqhtczw.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2spmniaco.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2acplbnfk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xtfknxln.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2hrpdimff.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nigwcyze.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2fphjbbje.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2yifitfpx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2igyhzzre.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2zdmibmio.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2troeqrou.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rfwalghw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2bglkfmoj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2qgrieeze.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xwvxpdkz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2lyycwihb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hyjnkztm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2raveqftg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2stdgdyex.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2flammxei.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2llizczoq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2chcwodjq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rvuibgfi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ifqphnoz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2kdsfhqrd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2irhnwyey.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gfpgxunc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2uklvdcoj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tjjhyrol.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rfnokauu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gfvpphed.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qwxuiubl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qbyklsav.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cxdkzkmn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nfynhpdm.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wxknwkap.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2aypjwhko.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rjgxxstz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2bhpebzii.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rnkekqpd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mjgyjqkc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2agrzusuj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2sctdacqn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xuxmtasf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dtfjcadz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jkctxwoi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2yegkplfl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nntrzrqu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mquotmnx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2duekzkfw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2juiifdmr.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2hconvako.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2msahjwkg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2abmfqoye.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pnyntscy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zufpvlxo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eufzxqhb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ppvqrykf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2pzkfdvth.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jkgvlbzv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2taezefor.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tznaroqr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2chhuffwu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2vvzadhbk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2jnpnumar.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zkzhtvey.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2glkjggwp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aybaipop.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wjdfells.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qhhqxybp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rmxmfjuq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rwicqdks.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tfhlqaye.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dxvkitxs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ihdodxtv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2lxvndxip.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2knzluqlb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2nkrvrqkz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2hfbpewqo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2etbhvgil.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2migrgoab.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bbauwjht.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qqjysfjc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iwqlivrl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rlsjxinf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hsrgxjpd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2secoxafi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ucbqfhom.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2alrwqdoe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zuzofjfv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ygacqdfs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2lzkpllcs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nnbxcvdu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ejspwggh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2sjbaopbe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dvmcouzp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bxrrlhhx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2bgfprdbg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rrvrqsmm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnkxsmo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2aapxwhip.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2zarlhhsj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2sjilavud.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2bictegnl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gtcvxmly.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mnejrxtx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wbbqvxif.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2fjvsriak.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ohmhdjsz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2zjsxrzrf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xyquhcgu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2rlozhuml.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2abdvnwcu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ixxhxdjd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2sdshkezi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2oolnkfdd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vznbqdpq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2gubbismb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gtyycyfm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bemqjugg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pduehnfe.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2uiuwrtau.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kyaxetep.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xaithgdd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hasjtdmd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ayffztfm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jhhxyiky.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nncfxuud.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pjcbcyzt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hamgvrbn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2zynhkngs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ceidywqk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jkxrgwat.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mytbviqs.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2nwhbocnx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2soworntf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rxsowqsa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2pcrtwjvu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hezzukmc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pxyzqeca.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2jrjvwgad.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2mvwbsrzv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ogribblx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2itvokmdy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2xjsgpmcr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pclhsodd.html


<!-- 参考信息 -->