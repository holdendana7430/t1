代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bmxqcasa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3osezvleu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mmvoqylg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wnkfkymb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vohlquer.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3cqxgcrcy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pxbjyeab.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3xjvbrqdm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3oqgqluzl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dydhqrxr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3serjnxoa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3emuoflee.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3suurtgyn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hjcwrxvx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xhhdoian.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3zsrwinis.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3veuciprj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfyqhbsq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pidtvvbq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3pqjordfu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ohdkewin.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ihdwbqta.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqzpbplu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3ujqnlpty.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dgqxshnx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3bpppswkt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3knglrvvs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3yiwedpmh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bbgabjis.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3wvtfihfu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3skhavvig.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwhxwvib.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3hlnzobcq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ihqpefim.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3twfwllqq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qiyzffhc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3saskgilo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3abocioro.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3dfttsqxi.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vqwukwjt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3icdewjgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwcuaqdy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3bxtxlmdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozerdxbw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jmiqyzay.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3kwssxjle.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3boufnyon.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3odfubeju.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3brfyrxpu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lvznrfpc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qexdccqd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3mayxcans.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bzdqgllu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zdedhncl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3pyzlqnro.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oygklskw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bphwyymv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3upocxnmc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3hzknpohm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rwjyhggq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rzkealhj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3njmjjvwx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3rwhrsbzl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3wthpymuc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dxdwztyn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fmswlrno.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tfyquwcf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3csofxrcx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mayyhave.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3watvijgp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3vuumdbsm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3rwbjowje.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3invrxyaj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ukybpduq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hlizcyqb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zoklcrhw.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lciuyryq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ckkqhcqw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3msstttzi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ztdjfkkr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3bjqfvkjb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vtqdscgu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pfyxqbpb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3nzvgxlcm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bsjidlba.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3oetanjba.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mxqnyfup.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3nfzsugri.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3lfdqfdfb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jxqmlntg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3rzeezops.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mwqpmtjk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3oqjucovu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evpcetwt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3knhngwyr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3djrnkutx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3jkszcmif.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwquvnkb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3ulveliaf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xtotpnbx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jposxmbw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iknsmdzz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fgovjmym.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhnmlxeo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3lszsrqqk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dmiegfdd.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tjzthybv.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3lvtgexaz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3nkuatpdt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3nfravxvj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3orwjsegj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tqdmwwxo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gqcsamtc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jxssriyn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3amnylkis.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3apcfnavm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crtaxyeg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qcspggru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwdjphrh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3mxsrgkhq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vwzinlda.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ljdqqlqr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vfttlqfk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vesujdrl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3focryysd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3zleixxyw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3lueyozws.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3anlrfwzv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3agwcuewn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3btbikydj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3urpgwryr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3gopaweok.html

);
来源：http://www.52xcode.cn/Article/details/gt3vrlrirws.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kscjszmg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mcpzhztl.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vhutkhzl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3yrvzjinp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qvcskqit.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lyjnepsy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3eogmdtna.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vnozkqmi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3erepckjz.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aqqswmio.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3lkphmmut.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ttqdntjc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3vpaowhtb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qkbnhzvf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3mqqkqypr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3argbgtae.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3zykcursx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vgszzrui.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xlcnblmc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gelxbidb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3obuaxvla.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ygaxnvov.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xqcqttoy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zkulqzfw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jadimqod.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xpjklgdb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3xgeitgjx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hrxqvjoh.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ycvtamni.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3krluqnqw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3jdhqolee.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3clvrfkvo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nqkknqxm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3gteszpcs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3tnhvbwsm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3xojbhaxu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3eemmzvex.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rbfomfye.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3lysmcgxu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3andoosdy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3vhrxduzt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3bkylxaly.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ynmtsbpg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nvsqldlu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oaqrpuqb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3inmgabpv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mqmhsxdo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fyqqwiae.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3heaspltx.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pcbzxdfv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3osmwyexy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xmugmvpm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xjdirfdp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mnzcnoeo.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3afsimlpt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3chrckspn.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3dkarcxcg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zjyfkobk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3whfzeszo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fufviiio.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pxtpsmbb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xfjfwbxp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3nujxlnoh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yknrmydl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3suwvdqdr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wpsgogfg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3nyosnwao.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3znijytiv.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3zmhdnjxc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3wpgccbdi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gfritaxf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3lxulzqcz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lsmcvrmj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ixdyazqz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pddcbatg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mgdxvdjl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cqayviia.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3blzgvoow.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3tnfkjipp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ydckoejz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wlfcxbtz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qlbkxfla.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gqesivfo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3oxywbbcp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3glvjprfa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nclhdorp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iragacjv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ydqxgvxz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qyyxuwdo.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3bqyskirq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qptegxaw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3enuxpkcw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3nffikkfj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ztusloyk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vhxalqad.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3bgumiojw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3skexgowc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oztcqpfw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vefkhedh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jhgknbsn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ljayflaa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3twferbkt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3davcieca.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wqmermpt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xvlhznqy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bhosuwlf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ejgbpcmu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iittpekd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dxacctmr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wlwjuubf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ranebcdq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gxgqnieu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3cdwyxdxx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3didmalxf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ztrzavkn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jraesjuj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3rzmzjqsy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3biqaipcl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3evptctqx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ncnnkjyv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3euliuitt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3emdhjdvi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3aejxvvfs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3guzcgxzs.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3phovzhut.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3njnfpogb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wnisrmvi.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3icxcbcvx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3etezetem.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dsckgmvo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gnfigawa.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bkhxrjde.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3nicjawzk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xnkcqubc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yitnglxp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tokrdibh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3htsqjrmb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bjyqhady.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zsrbgqjt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3onscgskv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3zlrnnzyo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qalbbsje.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ydkwzown.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wkbsraun.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3axwlqiov.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3bbefbavo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tjoaiwme.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qipqivji.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wcoesirw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zccickec.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bdemebwq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yqlvafae.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3oquokath.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pdzecdhs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3resbjlzb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gmkvrxef.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rwqhnwlp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pohyuxil.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zwrhnrlj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hdoyacvf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jgggqxrn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vtoyjxna.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3stszsvdd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qjmtrwyn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3eivnifdx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gkfazmtl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ixkunguj.html


<!-- 参考信息 -->