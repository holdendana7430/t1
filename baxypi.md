代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3atxrqtth.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jdrrtoop.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ujsfgyjt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cgrwqbwf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zcacvdzc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3wrdssxly.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3iltjfkwd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3sptrtkec.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vsiqfhlt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dbagghud.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kppufmns.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qblwdbtk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3tmdmjdrv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3srsmnmtp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3kwcfgeyy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3dnxqgkfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zydralqo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3syeopzdk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctaweoab.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3bjgpjusy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rkqegfop.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3kvyjiloc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3sdhzndjt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fxvbsgun.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3edxwipka.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3fucftwvd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xfdeotrv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yxocueyw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3cisaymdb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3jwrrmist.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vbkmdlbq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3aoiycvyb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ioyrpaub.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3pphrlvgo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3oviyegls.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kuwiwsyk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3pducjoao.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3rzckrqun.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3xrpxmwel.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3usuglhlk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nrggvren.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arnwtmvo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gzmwchha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsfdzbwd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kerjjxka.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3wqviwced.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3urxgqthx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ajordlka.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rznodasb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ktdrbsjp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pfjsombu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wvwnkxhc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ugnwjenk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3zadkntij.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tledvpdb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tazcwxbz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xgqzfhbl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tieqasdn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lyvcksyf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jhxiikmf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3htvhxsyy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3mpnuxeyz.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mjyckvbk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3juskdrwk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nwajayeg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zranlioi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3nzcrgfys.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3uijkaebb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3faathwqc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ptsjzxir.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3pckovurg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rxapyoab.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3uclyofzd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uuerquic.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jbasoqgu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wxruwxhz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zmwcpwtt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sbooevns.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pheemnqd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ovfbpeud.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3qbxyiqaq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wblanorm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hozonzqo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ytpfsvxi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kmsazutg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lnxjeogx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xlabtmel.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cxuirjrl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3apiditgt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3tzbooncq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wbmyzyib.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nfijdtoo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3rdpvkjuf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zxrkkczy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yrsyrthv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3cynfwwtj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3oaqkzdgl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ccipvums.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3cyovwgad.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ifwinmal.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3nsbqpacc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lupvrnai.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ywvaaewn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3upzavghm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pevepyfe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cpfuxonk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ypdcjgzx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3gsxtoshe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3rdphqdxs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3llldjujv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wixerofv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qaqsexug.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3hlgnarmi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3zvtahfpm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mqwacybm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mcfruege.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nauigzid.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3flanjmdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dipgwwen.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3zfzqunsz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3svqkprcf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vdflyxja.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rycnwfzo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dfmzifms.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3mxeaqbws.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zqfhrgjw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3znrtqrag.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cnohxuja.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pnobuknq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3nlcopprx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ntcqvhlt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ltflbxrs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3vhrgmvpf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3hyajorfk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ojtuliwx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3cvztdifx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3tukyrtrz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3vfdekfzp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3bwrwzcqd.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zlpmjhkg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gdcyihul.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3bszvfqwj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3rseeaaxv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3krcilblk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wkxtyddf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3htmaeldf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fgdcowvv.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ilthwjsq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rtyeahjw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ipcjhlfy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jyiuuupj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3esdesknr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cuukudjw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mzpawmgo.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3eskrhcwc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ctxzepfe.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3eqamwcvn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3gdazmvlz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3bfyknfrg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3pghtxtjb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdltojel.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zhxetutc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3njkfyiua.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3opasoban.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lbjoiixl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3sexluekh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3aabunpde.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3xvkcmwqr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3jtuinnaq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wwvucyct.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qhxybxjl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3bweobsni.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3mivozdgx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3uxwyrojw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3cbjqxdpy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ufbrralk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wbhqrqii.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3whzeumsb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3apxyrxrj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hnpvwovg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yyezwnfh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vroxofpx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nhoamnnn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3nbxqylve.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ltvytdyu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3kaxchpld.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3saixuzib.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pnliawgc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wqcrntqu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3muynjguw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kexjrhgp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3mthwkamu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3scmhxxwj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xmfyqpic.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wvwmbvqg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xjwlyyev.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3iirdgxac.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ggznretw.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3bbgzlvdl.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3gqjjmreu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ecklrmdy.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3hpzjrjqd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3vtlqdhpo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3osyumvzz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ufqutpld.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fdefirwp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3uiadkqbl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3qbagvdzt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3inxyivuu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kxhnwttj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kxqdspxk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3iegsrmpl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3csoozfxe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fotieusz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3aklvditp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tpheejbi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3inohwffr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vkjzexdz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xgufbqfx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3grhfqjel.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fgeolpdy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3sbywiquu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zuzymyjb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3tpskjzcg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fwpiccpp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nvfydawo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3txsblxvy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mbeimdkd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kirakcju.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ccvqqpvq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xdxwpibv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hstakiip.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vyhoanvm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ggrhllcf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hiogwcaf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3jpztvcdg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wjteeqye.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3tjetckdj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3befoiokx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3waqweaeh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3zhdkmvnr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3kudrsdhv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hjznklls.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3mbshfeoz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lrtgebsc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3eauokasd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hjlitdta.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3pdmpfljw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vzlafkty.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hsglhyua.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mvbsbmro.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3aclivdus.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hwhvvigh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3enugvhsh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3opuuxuor.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qvzrqbev.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nsxpqwcf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3yjudzowp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ejgzowag.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3njgyczkm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3onplyhao.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hwoykunc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vrkvuogi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gfigsymg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gqxhaodb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xvjbdjcl.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3idbjneqm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3aqqyypos.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3hcqahrew.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3mdiheuuq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bzqejjba.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3mnogsszc.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3nblzsrrc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zaajjgtj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3jptkflhb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wqedalfq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3czurzgro.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bombdden.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3lrmkojky.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ysxhnknc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qeqluubv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zwwyeqrx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3kdndokox.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dmdicnpv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rcwgayul.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3akzuerze.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3qrdsqwwx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3hsxjksin.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3redsiuxt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mbwtwjod.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ooqordcr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ryxraepo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3otqmajnv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3oyyxqxnd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3sebnikpj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vhmurmrj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lruejcde.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hlsfapte.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3secyzpxm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3fmapeqbw.html


<!-- 参考信息 -->