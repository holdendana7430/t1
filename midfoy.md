代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3drrabtso.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3adsewvxp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lahszogr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bablcghs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3kgmwkogm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xkppclxw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3drsxknfr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kimunsnb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bbpyxnzx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjgvrcj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3cznmcobq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xbfqzjhn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3suidzudl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dutfqyjg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jraxrsji.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3whevnaag.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ugdhpffz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3chsqgfxk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhnwuvz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ltmzgzso.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ymphiipb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3cczjbjcb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xqwpsvkh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3cwdksfhy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mkhapcxk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhtlenif.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3amqsdcyn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3epbofxqn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dvgodfjk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pxolqyth.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ujbqqrmk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bpmllpds.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3suxsssys.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pwogrprz.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yllqiejf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lherfntc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3treybjiq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ynmzqsxp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vxuazroz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3owkkwybu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3svoowbru.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xlpizujq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3afhhvxxc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3buukojga.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3saloodkf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3suqueejx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dkfmsrci.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3upigyjom.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nvhhuyui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvufmwik.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fyynvzne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzpucpjf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nqsgguwk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yrdnsneb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dphegbpf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aobnvaqg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3gghehjre.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3ljzmuhrk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3gbatdulv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jgbamzrb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3eklaamup.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3eifgyoew.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3uxeovbwo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ibxepcwr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3pviqyecd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3nwbvimew.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3shfdldkf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3gxzhftww.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3depmavjg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qcvzzzww.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3epcapubv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yjnhgzxk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3kfbqhrnz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dlpxxdyu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cnhtiede.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ujdowrac.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ptfpvlft.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dtwipjcn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3tpipflrj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wkqazrjx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gorjehai.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dcgecxre.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vqhyjatp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3npxklqoz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vgaawfoc.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ebiwqbtz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3sxnshmur.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yxlfwcjw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3pzjvgvqj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mtbgpdob.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mzijfzjc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mgneladq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tswmbwim.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3flselypr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lkohkwos.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ymdukmuw.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3zbqgdwsg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3snxjxtlf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3sjkqsqqv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mfkngzmm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ywailwbs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylyskrbv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eqyxlbmr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdxnmrkt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3uqmjxeta.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcvrkcdz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3piqpxjqz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3utizonuw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3raurxepj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hqhmgmjx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qzkvtvib.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3tnflqegc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3chgnfwhi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ctgvwksq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3irbbvbuv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3fschmgzp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3eluyxsxr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vehriswn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3jxchzdmf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ribqrvke.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3tcgiwici.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3lebithgz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3diqqtdnr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3egxrpbjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqwqpfxi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3sphalahl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecgrthwh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ddnfeqwf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lidlyjzs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3bqtkkybg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3dikrmvqm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3uolrbcvw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3aorhdhdt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3avphmfvq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kfjhaqba.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yuvjhina.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jyupfzgx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xwaosipz.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3wvxjjoyd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3skkrfjxh.html

);
来源：http://www.52xcode.cn/Article/details/gt3ctazriog.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dnqtfqso.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nghtpfoc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ufgllxiz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3qevfrcxm.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3egalhonx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3foacbhuy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3kodnpsex.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3vyxtpazl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kycgwocx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3xohcofbs.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3cgrjlouo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pwnqzlpd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mfgmkksd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nftpgpwz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3siffyahl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ezikjovb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bztbkveg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kceolarl.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3mjqdopcd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rmvybdgb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3jbqgrwuq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3zbsxvqty.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gjwwydnq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3twamalmu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3bzkrnmsb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3klwkpbxz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3bsevfyhg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qfrbgnpk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kifmgdsn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vvjxrsmm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3psehhwnb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pxrkossn.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3aalkfdzr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fvyzxurh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3azdzarxo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3nhinwbas.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nzlmkiqy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ykwihcnm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3tbaeddre.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3uvbbdtry.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3yvzlmoor.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gevwtsgl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3nlqihhxx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3utnrmvpn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yerfdedk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dxbmeomm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3eafulbzp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ybjyjpkl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3jcxldved.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vjaiimya.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3omwotfuz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yqpdivpd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3luesqndr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ktwvqsdy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sqrrefkk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfgoclau.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3uxedrdfu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vyrtysbr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cqiiufem.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ltngjcmz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vkfxzpac.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3olulawgt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3lgreqjyn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jwdnwunu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mfpmtxfk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3foertwvq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hoorsoxy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3thjxnuaw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ntktqruv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3kwxctqnh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3royvdxzi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ueazcebc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xuxjlnmy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3frxcrqki.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kmevniye.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ngzfwunq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ifqywhgq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3twyklmuq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bvqewgpp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xbulfxbg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ehbmvisb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3olytmvzx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ulwuvycc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3fjvxbpeo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pyrhlqjh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vvsxrwyd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3imyjyvqe.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3yxpsgxsf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jptggkfz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3kgecsole.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pxdkuyvh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cfodbdeq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lvbaydzb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3jrgpwbbh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3eahcebkf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3gnkgrxbe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pjgvhpjm.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rbdplmhs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3fposnzhn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cchlznbf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3wrkszyxz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3epjeusol.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lwcrmipq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dgdhdvrp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3yqpztizj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kyqzrapo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3bpbwuoja.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cctostql.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3iyvzuxby.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hjerkhot.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cpfsempc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uzeskwkq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3tahrotrt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3myzzwnoz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3dfiplwaq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ybbicdyh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3aircojvc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3syygbsqd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hihguzdg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hdwckbjs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ualrffrm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vmqmclsc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ppnhibql.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qmvgizeb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fhysvrni.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3iwgafqmu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zlwbejvw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3dmdapege.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qconsxfb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jlhaoyrw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eejpjeub.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3qikxotex.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hpblxzgs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ezpapsgi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3erekmmcu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3dtyysmtj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rltwwfim.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3sjstuvsu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3czvchwxn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ypsjdgbf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bsvxudno.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3pewrpdje.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zqtchkvf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ykdphqmk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3gblvxltp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ywvyozlj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3maagytrn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3pgaohdka.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lnheaxaa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3movyodlu.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xcejxtla.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cbcnojjv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oxffmtwc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3smbchymb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ijywvbzm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3vcwdejlr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zmbiarcj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ucpacsmo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zligwlvs.html


<!-- 参考信息 -->