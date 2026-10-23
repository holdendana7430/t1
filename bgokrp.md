代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3llpisxnz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pmpcfzud.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3arhehqhq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cozbarhi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3jemltglu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ccnojyfh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3opedhhir.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ovutjywb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3odyqbbkb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3aexivkyb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iluegrgy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3tsjlnuxr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pjankxxu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uvjepdku.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3keuotxug.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wnfezjwc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3dxenavdh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcipflkk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3woxebord.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3bacuzkmw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hrfxdomb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3cyckwoxl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3krwsyppp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3dckhgbcl.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vanxdemn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mbnvzvpf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3certhkoy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3neulfuto.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nvhhlqoj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vgacvlav.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3nzjpuxvv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3fimmixhq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qrkrxxhp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3roltqemk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jrseqrqo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sxfrxmlj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3trtfhkse.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3qbiviuru.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3azxyyimx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ihuvbgzv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rvvtdlml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvleioiz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3jkgynock.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enkaskhh.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3oyuavxhj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vwbiwypv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zgblhnhk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3dlkwyxkl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sisjktos.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nepsqvsd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3klhouogs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bkvsgtjl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3xycosqnn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wccttpha.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3emtxckcn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vcpeobwb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3roapgehe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3gdffivsv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3asllwaxt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ifyekytl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tyxkfihr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3hkeyacng.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3riasegeh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fhhalvcq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zaxiqsxw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jijgsesu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3neluqezx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3aydeugbw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3rfcsqhnc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3sorqzxvj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tgbwrswm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3dxsjcvuu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3bzpuqrdn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gkzybmay.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3twkraooe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nsqvaoma.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yocwvhtx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vestolgr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3sqvacsrx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mgqhweqh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rrbutcbx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3bdesbfri.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vkiebren.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3cebuzvzb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ypunjqat.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ontvptxh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zfujogfh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yorninsb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xgqrrkcz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3pnbidgoe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3iysbkeyi.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzvevcuj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cyusbfgt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtzogmov.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zwphctin.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ixbmlsmt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3gduutakf.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3oltgsabk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3tdqhgnmj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wywhssbf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3rfrgaihb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dolzvizn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3scaaotgd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3byyiewtd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3zydvyllg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jtvupqhb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jvybichk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3htcalumt.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3qtratobj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uyzrjhtk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ruoteewe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3plejbwxc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3nrdfparh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3hmfocjwk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3blsrzfeo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3nlcfchuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvgkmzng.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3nuoqlzhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdtnitrm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3eehmwijx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3xttlxqyu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jlrxjeov.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pabagdjh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3jswuglse.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3pfdehdvn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cqwroqas.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ckwhnqhf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3pbclyrfv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lordbmgg.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jzwnlqea.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tiqyxqbz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gmqbncqw.html

);
来源：http://www.52xcode.cn/Article/details/gt3mqahpawt.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3eiljputs.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xrsvmqfz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3bdsswbxg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rtjmznuf.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jqndefjz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rsxdfeym.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vwbpjruj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kltmlepa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3tygyufkj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3gwypaqzd.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qfrpsafk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tlvtzxae.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3lbyrsaqi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gsbakzcz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kkfgaskn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3chcnruzs.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3cpimukcf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rzhvmqfj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3juoksxdd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3kjeciujf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mnhspppt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3zbwebzbe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rwxgxivw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3avznjngn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3kuyenlga.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dzpifuzu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ucbclcdf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjwewlvt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fwhoghbe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgalijfd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3uajhmapq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3texogqqk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bkeyjeqg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nyynktcq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nrmorfey.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3mbplvnac.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3bjpwxsys.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lvzitcth.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3vlqmomyj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cwtpxbcu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xudtjaiz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ybnipmgh.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ribaiqyn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3pbjndyio.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fmtkwkjv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nilcnuwx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3utjiewvr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3jdkhwamh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ypjfqsxm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cyjvcykf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wtssoxyw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vysniykk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mwgmfezg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bwqrclhi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kqykdtjf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lkmyyupi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3rwkmkvrs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yzjvlzvc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yedskpnm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gdfxfcms.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3upbjiuag.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ifacbqio.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3oazgzavt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3xvvovoxn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3syjyjadk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gulggjxb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vftgwyvl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3frbcddfw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3wnvhcgud.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3fzsxfres.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3nurnrjjy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3epfdcjll.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wjxbayiq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3fypxmhqk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3etkckjdu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3fiktjfwt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3pliisiks.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ftcaovgb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3mflpupcd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3foykyvgu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bgimnwio.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rkizcnbz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3turjloec.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cwowzsbz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3twyjcrys.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mzeeserp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3jnogewec.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fobdqmka.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ptikjgci.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yjqsfmuf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3xkvnlwjj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yeezahmp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hnbpplib.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nervjqyn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ecbggdja.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3kdwvofrk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3msrpfrxc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wvvjtiph.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3docftpbp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jqgncckd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3aqxczvng.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3abkcclbk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zewrryep.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pjqyxzvo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3lwgyipqp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cjszyulc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xmxcrzgi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pnuffytl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3wounrjgy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qransskg.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3fnygquuo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3dbpifckn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3yxuqagrv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ukrvcsps.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3drenrnon.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xvttaxpz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ekxrucio.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jmurchvb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gbebcppv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3odtbefvn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3pjcoprja.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3awtrxekt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qbuoeyla.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sxetjyfh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mrgqcmbr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3uralkqhu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nnoxgdsx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3akcrwxpu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3riefvvjn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fprtgvtm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yxulygky.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mukgdkrp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gqqjzlgr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fuimeehn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3zfcvhrgt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3nogkgnnv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3szhuteca.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ljijyupw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3epleramo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ghmvdsbs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hzscfzba.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3hgfvfoiv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ncvobmlp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3jfmoqvoj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3cycvwrbp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ddolruvv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hiktahwg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3eroxtddo.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3fbscwdlj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3utgoyflo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wndszymv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zctajzzc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3utxqyyix.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hxitjbkg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rnapumjc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zrsewrna.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3erwwqxsz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cudzscio.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3trrnzafa.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qgsdlpzh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mztysyrv.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3meyjjlsm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3jqybyigi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3oteabbit.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3gemvyyjo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dyknlhqy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ctlfgrgl.html


<!-- 参考信息 -->