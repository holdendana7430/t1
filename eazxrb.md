代发 wailian999

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yjkaxkup.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fiwotjzh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ragdoqfj.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zdntfamj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ihttakyl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jqtbdzuc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2haaysaxi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hrhzqnov.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tgcbhape.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yndbbtvf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eojxqmqq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gngzodsb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2niykzyzv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yavrmtfs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkndbzlo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tsgxpqmd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2npcmopnn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iabhmcge.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2trjktlbn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tqryllhd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2lakgnjyr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpkmoqkj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2oabqtmjm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qtceqqla.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qdilgijf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2pzwgxwrg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gqkuqvfr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nenkjuts.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kxgbiklu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2aevvvzja.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pdulcklp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2toexusfo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xiupslyw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ypmurvwi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vtmzlmrn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnovcfyi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jzbhzvdz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2efpdrhjt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2tgaunrvk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ioaluwjs.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hofihaim.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2efzomxej.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ceulmlkw.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2aizcnytq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wifhsldi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jluagqea.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2efpvwjdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuqrqyht.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tkkkorvy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2tzekshcc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ybroyjlq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2njdkgrav.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2itxkqtdd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hwhnvczu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2goagxxjo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fcfpilde.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2iugalwri.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ccpksbop.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uaozqpap.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tuxerikm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rgilgzva.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2teealhph.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dohbutwe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xdbumjec.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tbgtvqik.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gtocmmhv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wekxjnqw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2sxdusxnn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dwsjbdph.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hdxgijwr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gonhefhq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hcapxuzc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2mdzqbtqu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2xjyahcyy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2dhuelvof.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nnpmhywz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rpdzmnol.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mzhfkvgu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wktdgket.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bgtfdfsw.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dnseoudl.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2grgvszpi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ntdcgifr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yroripzw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ldystuuq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fsnndgjf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2nzaekdef.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xzzytgzf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ihneakdv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ojmmhdqs.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bfklzkvk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mgiditac.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2hewlbtro.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2lkjsdwdc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jlwsjukk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tprqfonf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2kbrcmrzx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hldxlfvv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axeqsnwr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfftxtlu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qvphbcnl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmnrldju.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ahxdvznv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qzptewns.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2xlirdwux.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vkdzmuge.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fajvnkwr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hzlrjqno.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pggtsdhf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lvnqyetg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2acsqagkj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2fyyzkbna.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cfyjsiee.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2fugikrrj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2tfgniojt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2cdfljgyy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2crmoyxiy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hprbfjic.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2kcmvmihy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ppolqsrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmcmatff.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2scrvumfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2andugcar.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2phnbqxde.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2gxhbtoxw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ldjbzdnu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2drklerxb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bgmrbxry.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2wluvozkj.html

);
来源：http://www.52xcode.cn/Article/details/gt2rmeszmmi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2egfrbfpr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2pwzdabmf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wyjfcxtf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ikmjuoes.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2vbbxykaf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2qsocfjjx.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2phassvhx.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zokgpqrj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cmarxypu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2sewzhtpv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kgouymfp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2amztfkvu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2shygdohd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2zzntkrwr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2yunbdmvy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xlvyygyx.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ahisylvt.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lhmyggjv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ukywcgiw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ijzdaafh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2cgbsrisu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hxhzlexz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2aorxfzwy.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2igmgulkn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ytfkmchd.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2bluqjhev.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lkkohisu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2zcektout.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2kgsjsujw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ukdjqczw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mrhbvcry.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ekxfetnu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hqjygnyv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vidgtniy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nsiyjugh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iqqvjhwo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tzaepnve.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2rlrlspvq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2zikfeocs.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sqarabfe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2yzzcflnk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2entxmlza.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qyurfjpl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2qnsayerv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ddhscwwb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rdctbqov.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ahxawskv.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2xkfstefi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2pyozrpoa.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2fldtqlks.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2erhpwadh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2atbnqcgr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bvlsnnxf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2glpwhyup.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2hvpvjkza.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qhhdrjgs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2afwnvhjj.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bntyqpkd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gsulefgo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qijwjhdq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aqkdwvvm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2axajqycp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vbenzpxj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vrcfdknd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wzdlsqmv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2mjrartgz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ivxwpjjl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gnusidap.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2frsedunp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2uvgdkzgq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lfggkysl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zjrwddqn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rwfvmjht.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hesmbjgl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mfzuqfxr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pgymedjn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jptoqswk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wwrppwhw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ubeucfcw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kfaaxzkt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nspyzvvj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zwqhkrse.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2fvfcdwbl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2hfiyhltv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qrlodphv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2vhfyincc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bhecsdey.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2iowpqlmj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xijxlsis.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mtexyvjn.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ymunowqf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jrspbgdo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2gaxfmqdc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2btjotbnd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2jasblmhv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zjepbrkv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2jrgashgk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zbdzrqvw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mxluykhz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2hjumwsry.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2bufsffsa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fafaiszb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2edpvaqwe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pohyjsvw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wisiqxef.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2hdkyuezv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2joiveryt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2rrnloetl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qxdvtihr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2puuojpwl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lersgyaf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2dwabbhsg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2usqkuhcu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2jpjwunkn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wfytilsi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tcrqnlmg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xtttxvhb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2dnzbxecx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ngevtnaq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2pudbzxsq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dnpgaebx.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2trcnyucr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wtpumcgh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fjjrguih.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yavwkewu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2sactdhai.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qxgrklyf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2johfhxco.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yedzdwbd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2cclaiwfh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nowaqcsb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2tfzdsqrp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ptjejiwd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uihyfvps.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wwwdztbk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uvqjqfes.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2pwypqidi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2aodkcjpv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xqsdtvwy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2phwhyzer.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2oefpwpnn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xoyubcsz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2methiahk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ovavrznk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2slodrakx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2pfferseg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2oizpngbx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ugoaducy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2brnzsrrl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2vweijolh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rshtcojc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2dkzngpth.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2uczxrure.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2lwsbjjhb.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2sezqrhmm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2fbgxkigf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vjhcbect.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wtjqxgvy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nlifqzcm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2cdqwyedi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dohwawzh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vkplyrsg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qqqeghxz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mgzjnpaz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ohavfkfh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2cedliwuf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rqseciml.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ebcrdgvu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2kuisotir.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gzzipzsp.html


<!-- 参考信息 -->