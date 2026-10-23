代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zdpokxyi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ianjxhlf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3wdkyrykh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3asxhiekc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3eqjvuhws.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ptormszf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3peeylgrp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3qpikecmj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vzoleclt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmkkjxto.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vcmdnbbn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3lfskyqrn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ciocwhvx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3onizuaoy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojvhniyi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3falbztha.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ykhmjfwo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ulxbobuw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijmpwavk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lbdiyrwo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vtgtosbx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ujpsfgvk.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3idzstujr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yxpafito.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xehbzobw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dqdbrsse.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ultzflbg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wclyrrdc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3uypcfnqp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ozxhffdh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3iangdhth.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3naaicybd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xgbfjmet.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3pnybsgsq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nmxjggli.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hawmohcd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3mjmtmosd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdxyteek.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ezaqzlia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljczjjoh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xqnwmjzq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3oealwzji.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qwnarvds.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wicoqulq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aszrniuz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3otshlgfh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pkzdyaos.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jchlzgir.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3doidntjc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3zniipvgy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3gatgsjib.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xhqmffpf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3wiwodbhe.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3hgiiwzpc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3urhaqbre.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3qrwdhbgn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3toycojso.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3danmkbrk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zgdlkujn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3svyomxuf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3kcyeyyhu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3elqopcad.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ainlatrf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jjgpvxkw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3mnplzucv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3tbyslees.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dqzkuhbv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3pdbkaaey.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3snwlosub.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vcsezcyv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3vqrlmmlv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3okoujznc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hdjlhzlt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3zzgqcgba.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zsseayea.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lsxglbac.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3kpqgrvlq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wqiasldk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3vcazisno.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3vecnobep.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rodnqacg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3iigkcsct.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xdbnrfye.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3jetmwhfe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3owsunntj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3yacenaef.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bahsxvkt.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cibsgqyq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ydhaasse.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acnzgqac.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tsaszwcp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzoiectg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3yacqbcix.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqsnnanu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hnnlttik.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3lclxxscp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ycfqyple.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xazrskyc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3agyyxkno.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hszykopp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vzyboero.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3bduluwib.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3yehwdqoj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vodxzndr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vyfqdiwg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3logofpvw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3tilioufa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3idwijhjj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3oaeghxbf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cyxzyiat.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3wwsdzflq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3kgszmzgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahlroxgd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3aouvfctd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evytatxm.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3stfpotjo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fhdhslnf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ypvxvqxr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qdyhpzel.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3mieqezjj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3fhrhrkyw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tleiibyp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ypgephtq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3vnnnlxss.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3fjcuofln.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ydwsanwn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3gewnyqtf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xxkblywu.html

);
来源：http://www.52xcode.cn/Article/details/gt3rvhlzwuy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ckticnxt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fswgmugg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3axsbyzgm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dxkijfvt.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zwifoyng.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3penfhwuk.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3incyugum.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3lgkqcaln.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3cbcgesov.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3yphadkkv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3inclbfwk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gmbeeufo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3fvqnktvp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ojtxppgk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3oondxqka.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xfubserc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3aichfnhd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xqhsxeoi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3lxaaqmbd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zaengchp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3fgwulkez.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3furcuumf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jtrxclof.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3mlpkkvxe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3atwnmswi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hjhlmnov.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3mihviyga.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tncjdswk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zwozojjg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ytmirtwn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3thmvlitk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fbrxthfz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pzuqjwtz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3xrucoyxl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3laqelkbk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3fbvheeau.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3sxjgysap.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xtkjuaoa.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3gimxvieq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3lmmgnnrz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gjrxvpxk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3enkhmjaz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3tzjvksbw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vlqpubyc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3uiofjcec.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3omucpfmk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3hhqcqqkw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wrwlvebh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wbyjzzkw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zmgqgude.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ewlagmdu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3okgfpzku.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yhgfmfvy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3arxmiedj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kxmygtgi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3avldsfod.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fjbpovdy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zuomjcrq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xltxumuu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3vjleryax.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eumxwrkb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tpqbhzsn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3xodrnugy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3bzdkfoia.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3goegdwjn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wwzvomkv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3qcfalufp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ycltdrtc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qshhfaax.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zglpqukl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gsietkqk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3hzzwwdko.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3zdnljdih.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jlspuqkb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3emjwmtss.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3siydyrhz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3owupqpcc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kvorgfmu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ocwwxicg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3lazaoaej.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3humffwks.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ungkpnrl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3xxhrpert.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bdsrrjgg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kncbufpb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3auowxaix.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bldphlmz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3bbbptjri.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3najoocyy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ihdossit.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uaimolcs.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jqhsjcgt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3rhraznat.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zgcorhjn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uqokzzyd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vufaaayc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3exllpxmh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ijvvaybi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3rijuzhlz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ompcccxq.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3reoqvrur.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3beuhamhz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3aoetmbwp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3sklxhfji.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qnzltxkg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fzrrrggb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3sbjyfnwk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3txamemau.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3tmqjorah.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wysytbdd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3snvsbcco.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rorqkygw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3rysejveu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3lzzegaji.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3myacujem.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3oqutyveb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3iczswmpt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gddejvup.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fcscfrqo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3easibrle.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3oplnxilk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gupcvsnn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3snecervp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ehfuqasb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fndybfad.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vuktmxsm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3stxrqfqe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3aadynilc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wfbebshm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3spnrlenw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ttpwiydi.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3qwavcqsk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bpnlraff.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tpedyoen.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3bmhmazge.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wtdtfzau.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3vyrwnibk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mvubchof.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gbseziro.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rujrmtrc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3yxibhkjq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xddhxhon.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3abvnwiov.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3luhlphfg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jgxowzyt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3muayxmdm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ogednvir.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3tfonhtfb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qjrvxxyn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3uytgkzig.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bhmxkzcj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yoaucdnn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fmutzgkd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xvvzneml.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kzqfayfs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ehilszwo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3grsbghcm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uymjujar.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3aaujaugb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pbboxyxy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3klpotovq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3buzoymms.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xqtvssov.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3klmfabne.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ucruvtwo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dfpttfhz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3qhjutccf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wjvpmhvx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jseytfoe.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zovepobt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cpcfzfvz.html


<!-- 参考信息 -->