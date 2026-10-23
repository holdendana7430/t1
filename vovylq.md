代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3oyltycrz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3vrummyhz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oboscqul.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zvfwzsxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3daofddwa.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kwncqfrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsjqikjd.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3gzhqbxvl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hdybvqch.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3kvugrasc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3rpewrbkd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rqgncgcv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3djzdvfzs.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3blhrcmfj.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3rmcdtvxm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3imddvwsj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gjkabpeq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jovwsftg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3mzdbggod.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cliordjx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jkvlmfiq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zabzhngb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3qoxehlan.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lbcueczt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tgsuzpoz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ycgjcprl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3panrnxvx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3lvxfpkcc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3qcmtukyz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3avwtvhur.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdulnzdz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3aljucytk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3yxbldjpk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuzotfcq.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cujadmrm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3stsfnscs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ntutolut.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kgmoxrnk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qdumyqjp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xchvjcub.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3tbjuqtrr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qgsxsafe.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ykyjqzov.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zawsvmup.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yubaeubl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jwqdvbhi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cljuccrh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mxlcltzc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ovtnrpkq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3djuggiyu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rmuyjzgs.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xuozbncy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ysadmgam.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3oqwsntdu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3nypyckrm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3svaudmzg.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bculbdrl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ywsiukhh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tavowsoz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3sighxhwx.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dzzrgjzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxentoky.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtuymqyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwuptktl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3crfrabid.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rtikysbi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lhbhinuf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kgseqlzb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rcbjuxcp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iegovuqu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3mmqqpruk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rteiesgy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cabymakl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yblhjzsi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3dbuqzorg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zsfpzune.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3jnqnzxbf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3iujzpfrt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jihvkgvr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3umuligde.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3imswutpb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3acabvhoz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ggejgknp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3udsoifdd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3olftxpbp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gpsypijs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nqnyubpg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3llrlvvdl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3cnotlxzz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tfwjsxju.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ktfvafos.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fstjginv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kzpulbcl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gqammsxp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ssoizzup.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tsdimsxe.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3umgvcodq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3rzfozxdq.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3byvluvdc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eqgxivkg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mysvbfwx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3qleebfxf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xnsfcwyb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mkwkppfq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3pdqimeft.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tlyfruib.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3agzktplf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3kjomvqpi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hanfutmi.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3emnjwhcr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hfdcpsoi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3gxipgkmj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3fullstxk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vljzzpcv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rlblfawa.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqerexcw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pkmgasgg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3eifarhzz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qwcxgrsc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3dnjlkyjn.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ivzyxgap.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fffqmxaq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pxbwkoaz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xikyiblk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xzovcoka.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3zwvrjgin.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3knmcdryz.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qqfvqnzo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3jfexzusy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3dnerzadc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bhsjgmde.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bzkzqmmu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3sfqavizg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3innwxfoa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3vgzfmftr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ugatymoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwucbxqd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3veeoknqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anvmbwbg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3glgwkqcn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3cmfqyryd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3iepukdep.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3eewqpiyy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bmoeadwc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3mzjgngzl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3djysvbgt.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3glmwzvfw.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mggexauj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3nmmvejqf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3zigtouli.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3eatjeycx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3acstynfi.html

);
来源：http://www.52xcode.cn/Article/details/gt3kfhxsbnc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ksmlvmbn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kmjyjckf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ezpjdrmp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jyelpnsk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3joomover.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pgqlryqs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3vqeblfzx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3klhctkxy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kpnkjfys.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bntxzkhm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3vkmkmmve.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ghynixsx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lpbvgbrz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3knevcjfo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3qgqjbmrc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mwkvpbdz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3tgzpgbzp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hnzrshoc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wswajviv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3elnvwyni.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3elwexfsj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ufbzrfow.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3kwugsqxe.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3bnwkjbjh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qsktsrng.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwblqbi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qywytqhd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3skzbgdxd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mvkjlimy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gjydbqdb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3femasmln.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xotwcsfz.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lwhiveej.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jwzvpqpt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3hnhccven.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3sdsslvgi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3hjfyuree.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rhykezus.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3njfhcjfk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3euduuogg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3khwsjfdl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qyfeguoo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3htodnjuj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3htduubnv.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3smomyclo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iuzpeinq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3lrfyoksp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hhewyswh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3vpxhznis.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yalpjudn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3kwmiohpl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jasiqwdn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bnkroveq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mgluqwlr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3edcnlxlo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kxhpdqxm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3anxsbvfa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cplkmrsp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3xadasqbu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sssplqeq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rklgibdk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tlicyiap.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3sfcpfqhu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3oapwfolt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3oetykgah.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3avxzqmmz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3tsleqcmw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3yuhuayuf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ybsatbcs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zuloadyy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ljzqjqmx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pteykssj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wtndiami.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ihbifsgd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3guudmdbv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vcpelxea.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gziczqcv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3pcazkqvm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3grqvobnj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hxdzwiak.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cuqhnkcs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dazylqup.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3lqigebtp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3zigzayey.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vqnpynua.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kjxuvkvd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ozpatnzg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3uehpfhwh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3nomtmmac.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gdwssvej.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hvxqwbwp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3umuxsecn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cvrarucc.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3sqlakpbk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pbplfasc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3xfsbybaq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gkpuowau.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fpreykyc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wdbkrmlt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jhycmkwz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kcuhlynj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yzkzhuqu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zqvihiye.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3snpcmioi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3joorcbjp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yrlykotv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3lgdjmuau.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kmszwowm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3vnfyuszn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fzpnmqkj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3zutqukbs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kovrwpkx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3btsacbwz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ueqmwkqw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kncvmoyx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kqbxayas.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3pgntpwgb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3aobccacy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3fvofzcbi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ewdmtgqj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3invbbdoa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qvbfuprm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qbopbbbd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mjuopwlv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wpriiiwx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3nipoejma.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kteegtzm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ohojiqgr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ijyzozlz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vfgxpebc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zglxnufe.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ptiouhbt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3fbxgirln.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3onalwhzn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gopezqpv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3gmvcmifu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rpwihqdy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xjfbwmva.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qsewiixo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dpigrjju.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3bdebihnw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3oufuyvfo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bfypjnmy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tguxerhv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dywvhjvc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3geagzbqv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3oumvplfa.html


<!-- 参考信息 -->