代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3oqsguunx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bluuryzg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3sbcyyqfe.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3oxryvgoj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nmzackvs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lnovdles.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3tzmfsdmg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gwoamzuh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cmksxpoc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3gdbromlp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3dqihtiln.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3sfknhflb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3sxapplnt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wbjvuepf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ajbdexng.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3cvjhxmpc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3otzjjimy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iuvmxdua.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3awkdvlke.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xportgsy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ddznumon.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tybycyqn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cusbomfj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hbbcwqfx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3tujhgwfd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xcvewqav.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqyounpj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3czgdqkeo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pniywyfu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ccfjcuro.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kavzqnvq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3abtmxjin.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gemavqxj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uudblwho.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fguoahlh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dexpyidb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ytzscocp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3skfizklu.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gxlonfur.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftbshjhk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3rsmtxyra.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3dnvfwvns.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3rjpwwucb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3vaxgsxpl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hvohaftr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jjnmefyn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hyjzpoom.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wndycbsz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3hmsypmyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylnezhbk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fsxzfrtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtznhqan.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vopghqzw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3nmqgacyb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3jjjppesu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3embevtoo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vggaskqa.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3jqvtpxfw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3fcpajlum.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xwupwuyt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3wjahczdi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3onzocoug.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3eojrepyh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vhztgzbl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kopvfkur.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3opfnpeti.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3atskwnca.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3twawflbw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zvfmzswg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wgpaypzy.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zpovgxul.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3mexkyhlk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3iennlpkf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jmuweccy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3osetmigj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3epmhjmfz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hjjgcnsy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3kdfwrtbt.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dzlupnbn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3scejdtme.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3drhfhhdk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wcgymkrr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ubrvwdsj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3yfckyfqb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ckytihlw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ynrtgtro.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3osohxwwy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kbandrst.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dnfrnrzg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3cgdlkbid.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3avynnlas.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3bxmlowwl.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jhwehwor.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gexazqcb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fptgjstk.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3tlerbfir.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3zafcqzzk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ubkbotit.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3dgqqturw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mclsdhpi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3eeaqhunj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjsgzxar.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzklbnlb.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztypyzls.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3lenqqrhz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zbidfoxr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3brcrbicf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3rrntrgdp.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3fmrwllqa.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3brdbxcqn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vdgqxjqf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqniozyh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dqqgmqzw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wnshstpy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xptgfdmp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ufoheoze.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3sgcxmvjg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wuherzsf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3iuijdpsy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3itrlwxei.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xqreuqkd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3arzklijg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sbwmbflq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3jmmqoabr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbqiesyv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3lgvmkqaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vijuvdie.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3dfunzwot.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3sswzkmrj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rrainpgw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qyqztkja.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3encqpqxy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3wiqaljvw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3dlhfbohw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3oakldusv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3gtxcsbcb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3lzmmskhs.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ftpmztie.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3cztmtptx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3enuljkzj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3umnvwkhj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3rttulqxl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nhbvysvc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3hpgeppai.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3phsrmqdl.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ypascpki.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nxolqcbs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3caljtacf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nbsnzbkq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ohgentbd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3zgtliccc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ftbsqnni.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zqfobmpa.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3lauxzgrw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3hdhunugj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ahkocnqu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xmlfnhax.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3qxrkpzpq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cnblwjuj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3gyqjldgj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3dfiwpemz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3xiewhnix.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3vapgshkr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tdhwbnmj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3onhtwvxj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3rzthnuai.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ccqmdfdm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bpzfduul.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wemrjiyg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jivnqmpo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3scjblczi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3wtqqrbfx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iozbqisr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3sugieasd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ntzucoto.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3iysjwrwc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ozhggqeh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3uvlouamd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cpzuvkuk.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3hyicsnhe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qoxirhtx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3webtzzpu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3oizjjtct.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3cadgsbcr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3mcloaufk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qqwghdxp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3arfohvru.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3hbaestpn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3rkzqldda.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ptrhzlhy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jcsbmfja.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3xfakrkzq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gjphwehf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3apvrrgaj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gtlxqyyf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ubovosob.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezqxduju.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3hryfqvzy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vmdkeprh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dntvisln.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3pjqfobdo.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3phnqvkmy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iirwhaju.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tbvuphei.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3juwrepwq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gbbrpxcy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3sxvecraq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3xvicpskm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qlehqgrf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dqyuahbp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3zoodinhd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3unhjimbz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3htwadsik.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rqiswjha.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3dwmbugpu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ejccnysp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3odgautcy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qlafansb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3njfkhrzz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zgoaexvt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ucxjnxqe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zhgdnqya.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3smrlruel.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3hwmubkcv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qulluqeb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3vcxdrkwk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wxnmmimm.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qkiykbkx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3plzohhqt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3eowjpbaf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tesgyblc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3yyxmfbww.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zbqhusnh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zufjbkod.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ulpjcjbb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hwuhksgo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3hvscarjc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ysphervg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3cqybtygp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3fbyuuixk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pojatqjm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ysmlmhmb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3etilvtqp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zrlpsqfe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wupqglma.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3yqnplelt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hdgzdeka.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3yjhvddps.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tieuziuo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ankybmbh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rpigpnea.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3dqrqcoss.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gblxllbq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3atdjpwfu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gmflpzlc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3umrboqrl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rqcqlurh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vbzvlvvu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3fwgdbaim.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zhlermeu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uozsxnrq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jyphanfh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gkljfrgw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wsftvqud.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xbqtxxjb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3uicenbsa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3nbqxbues.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3debuxbdm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jguavtgb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3byhdormg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3fhlqwceh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tiyelokt.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ngulumhq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3wycaoxks.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3veofyquu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3avfxorld.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vxecbgrl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3lpztnwjx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3koaiwqss.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3dsredlxz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3sgjthnvs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3eakvxqqu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bqbtdxzu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ojngaopa.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qxcbdrby.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ivgbnzeu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3udufzqth.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ttivxdjc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3osghpyjj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3klwjhieg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3fhiuorgz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3oyuuapnx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gnjmhzcz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jljisogm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ombbntae.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3fleonspu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mbymtjue.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mbbetoyl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yqixzcqg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mllycluj.html


<!-- 参考信息 -->