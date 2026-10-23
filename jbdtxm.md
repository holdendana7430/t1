代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3mcnyyofj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mdgufjmw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lfnlkyzi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3imgwhrlq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mvytsydf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3fjumekae.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vdkypwtm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ipvmlbeq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3voqlzmzt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3svqkuldc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3biydylet.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3raexmitf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3wklwugpb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3yandwtzf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jqnywbzk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ijjeubin.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3rrztapkk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3soumbrzt.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wqytfpju.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cwrymvhr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xnyvopqy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3shjcdmlu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qsaopqbj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3aysqnozx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jwpocplt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hsekkxiw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgumhsgd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3pxjyjdjh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3hotxemwe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3eyujlujd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mszmtsvl.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3lmkzszeq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bkdyjuxp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3wvrxflpu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gowltabo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eveyocnp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3quxketbd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3fekooybp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3bjfankrv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hdbaisol.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3bxjjtrer.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xefsxszf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vjzlycoh.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qltxdjgt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3luhqtvgb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3xyrbeeha.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tknrhngz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3kwfvcrxx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tuxjacbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhumkkmx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3iutwtgpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krqaxmkp.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3qaxstnjj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3fyvxsyhm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hopsztqg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rdoacfaa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3asdggecz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3osxpfxvi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ydlflloe.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3uahbrysz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3wjuihcmo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3cryegtex.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3osfckgng.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3iyyehwsc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vnkspaxs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3krhxttde.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uynjaapo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3xnsupmgm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3dzvreern.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3iuydxvcy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3abbepcvb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3byppsuvt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ptnvfwcm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fwrplcud.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hlfeojgb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ouagbmti.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3drgtfbli.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xbwqhaxs.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ykybarwd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ktnjuqgr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nxyhzkpz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lztswffk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nacnapfw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jlzjsdme.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dqayzwhj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3lqyrzoal.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kyhvivcc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dhabeawu.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3cisyvisx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3pkzdmzow.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dwqtjfaj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3lfonzekl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ozigwrkh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ttzkvczm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uwyijmli.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3lnnnqvxz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3grspiueg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ecnidwdi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3qnqhmwfv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kncuqmen.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hpusiakd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3boevidyb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovlsiszs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3nzpskzgv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3npohrtnx.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3wmbzoalz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zagfohwx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gbjdajay.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uazozlbf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gmivjomp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iolccbnr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rhcolsmu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3zuwjooxc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3blpkwhok.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jkgvacpf.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jbjefvcv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3plotpkzp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xqkpkoya.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ylcgldgx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mvzquutp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3ptipszaj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qggbyier.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zuveefkf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3njowotbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqfipwef.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3wcjepmyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfwnektn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3nfcnbueu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3iikxqpve.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dnwoxmss.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bbmfxhfv.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3jyuvdtkh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3cmkjtacq.html

);
来源：http://www.52xcode.cn/Article/details/gt3zbldtuoj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3xtcfieht.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kqwoxhva.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rjdlbffp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wtrjtacd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3noaghewi.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3vntglver.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3rqsdunrf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tqaqxfdg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3uqcemyav.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3vauglldx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3frhlbpzp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3qnievoyw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3punggfuv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3prqnnlbt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3cbobyoio.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3repwygae.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3aylkyvxe.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3kdxccgib.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xehdcobq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3eupcgmos.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ynnazwgp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hsucpirl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3rxfkglcb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3iqrutxcg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zbwabxnm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3macuxhto.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3knmdimcs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3eczjnbfn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yspuzuxe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ogtnkudc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3dyxgprng.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3lofomzbn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3xhdflcpc.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rhuvrhpr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxrmdbay.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3fptfszuz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3igjqncus.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3qjxmlrwy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jnujeqvg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3baowmtfy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3jdkbkmjf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3kwwjdkui.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3typrzjid.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3igzajjyg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3brvbipke.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3exxdkaoc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3baixvhrk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3rmgxcymn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3rqmfumqf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3sransymv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mgzjqghv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3oetegizh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwjkieqn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3svnpwctv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3zqwwsuag.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ndvhigpr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvzloyhn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tqcfjfxx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cchmgflo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3engjizkt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ysdqpotb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rjfcgili.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zwnvfcwv.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bfhqsxhq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uyqaidvu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lvbievro.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3nrdqnmhj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sbxdmgte.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nwjpispw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3yethlibx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lpshzlov.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ewtvwjvh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3yhswkkfa.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3tydfsxtg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3wblxsemz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3lbvpijlg.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xvzfjpqd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qkxocwfe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3tuyacvsf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dqbdmjmm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3zclgbfnu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ymrcvlkr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ttvdaywx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fmpcsorv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3joisqktk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xqvhyroo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ucrsuafy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3fysjukez.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ripggoet.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3miurnado.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3mxdbbhfp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kdmcfzlv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3mwcryptc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pjenjuko.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gwekjgqk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gusntgqp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ypsnpbto.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3gtbobzgi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zqxlqhhc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3pglcdghu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ouykqdxy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3douvtfkb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mtqqulxp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ndddwmnb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3isvoaqab.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3juqfdobx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vxvhxvuy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lxaqvuhd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zgtzdzwi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nytcaadn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jwlpaivw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mdpzaoih.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qlteojui.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ceidnggc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3luzrlpas.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vrbxulnr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yptqaumj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3wbamxzfl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wzopwsdd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vqcfxhdd.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ddvxiwor.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fqlditcb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3janidacp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xlbxyyeh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3durzopsd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nacopacz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3btsihdmo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3oakbvjai.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3thxbzhyc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3hbljyhuh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qjosssih.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ynpoyshr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ugtphthi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vymijhyc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ohgalrvt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lfqygwkk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ekcqxlod.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wlywsuzu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vqkpmxvv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3vcnbecth.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3obcmmldb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mwpgrozj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qcvmkoig.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3inddypvs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ajfguyva.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3delqvgim.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qvzjwkhi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fphkquei.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3pmcxjqab.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hseubasz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3afyfkwqr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qviawwyw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3alacgsfs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vlzubhdl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jvrenznv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3veidiczh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zgytcryv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3anrikosg.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqusvrjt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hlkaiuvq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3isqzrfeh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3czmqufqe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3eoevjoho.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fqbcgywm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rpyexmzx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3hkdyhgrz.html


<!-- 参考信息 -->