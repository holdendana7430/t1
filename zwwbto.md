代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dujkzcbf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2oubqjupg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2dlzgrsne.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pfjtgcii.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ozgxsdqq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2dodparje.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2idunkegt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pvmhpgwk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fkymeaup.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2biohloxs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2imrghkns.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2abniucyx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2exyunoey.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xvgixhjo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ffyfiqai.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2domfqvcy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2uytkgwou.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jedrdqwb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2eobctnim.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gwtfaqeo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2phsjgxrc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nnkbdwhx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lmarhfpv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2krttuxvf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tfdjzswq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zafprgce.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2xjlglvzh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kampolcc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tgbjgorp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xrguidfv.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqtylmmb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wkiefuvd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2kldiuxqm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jtfkgsyw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qpveydlr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2qindlqqe.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ofrcxcog.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2rkvbmfmd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2imrmxbvs.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yslwtguh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2aopjgaqz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jhcqifcj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2avqwzbsb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2nlfwhtgw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2svjpfaqb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2mfkgusub.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2urftrkzq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wsyeekey.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zwyvclcn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qbmasdiu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2euekxrnt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2aqogfzos.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2oprdkzkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbrebeqk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbynhzmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yomkfqgn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nobpqfvt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2oendebeg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2memlhtpq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zlkxunub.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2esncvwre.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sdaqeodx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iavbuzpd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ffmkomhj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fwbczcuc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gsrbfxjr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dpzgvoha.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xdhtpvgj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2srackeay.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bbxlsjbo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2upitkkyy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2lrcqfllk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2cviqqong.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lizltoiv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gykddhma.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mfaeflra.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dhqqbzqc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mmapchdo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kqrwsuev.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rxhksyzd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2jyegdkds.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zboigpno.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2frqnimqm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2onicpcyj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2dyojhczw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2frduemnt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ycdhecoz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2pwhsqcut.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2menhkqlc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ndoerswm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hsxxundf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yrjiukww.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2kasebxoh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mdxvevjp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ayrqefjb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2azohsyek.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2klhduefi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tdqjjanl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oqkqvpzr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ipkbhsov.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2azzzxqja.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2xivpjhit.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2btpaoslz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjifbpox.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ttrfybhh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyimayox.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsozzmga.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ninkajgr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2cbmittlu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijeazkce.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2gspvyjhr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gtdeagjq.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2pswrsjsj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ydbmynli.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gjovfrmt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qazyfzby.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jydblsik.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2aeouryqz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2zizkkxgx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pajeufcc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lcpdijiu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cbgswmtb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2vhytolbt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2leixogkk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2wlabvalj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2klqujupk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xdfhphid.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kkoizqoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tggljhed.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2umlckrhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ueoxktbb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ixqrhxeh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2mdqqkeev.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kdjyxqik.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uifikxfa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2cghgjaje.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2kbucovck.html

);
来源：http://www.52xcode.cn/Article/details/gt2qgzattgj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rrhaqpsi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vdabymej.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iqnjiefg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2rcqtkhpf.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2lsldahhl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vudyelsy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2jmbteysz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hbqfatqn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2vhrpehxa.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2jlaqdmpd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tjlvcslu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mkscrisf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2idcwbegv.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2veacowxk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2eiidqukf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xqmjnnvr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ijtuculp.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ngvftfcv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bwyacvwu.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kulnlxhm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2vynhoerq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2gppzyzxx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2avhxvpbv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2lrxotxkt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2qsvufyvs.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2gntqfiyw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2gogimhvp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2efjhlaxn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2pudpmngh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qjwwoerx.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2sqjhkpfr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ntzeifmz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zschzcdp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2txyokjyg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vjybhlly.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ynidcphs.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yjccpufy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2eoaxepll.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nzykdbpu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yititwmf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nnyeisfc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2fsmgpzyr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2uugkmfxt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xxpgkbtz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qobpjsnz.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ilzerdws.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tyindtwt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lhqbhzma.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2buhlfaju.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gukdzrle.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ndyhuyeu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2amwoifkn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2epmduhoe.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2pirfmquz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2bhyckswx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2bmjejjuq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2plpqnpfq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2tewlfpac.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jgxlthxq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2owdqdlhq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bxugceji.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2euteunhu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2coqxbgxv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2veuhfxlh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uqcdfips.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ircvatam.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2msuahosj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2syruydpa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dsephnvb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2iadvqqza.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2oeblfkad.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2usrvotfh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2fzcfsmah.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ximdfllp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2jpiwvgii.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfftuihw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jkapckha.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lbmcbnwz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ticmjhru.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nyiflmrm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2oscngszt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hkjvvrtn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2folkipgk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2obcbbhid.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2dfunyueg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jvkykyet.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2zisjmuli.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2rpblxido.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2jbtlizzt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2cupfjvlp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hpqfudhx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2fytpvmyp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uuaeuzni.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bifdvczs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ouyfizau.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xdaxdilc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vvgsbivm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fecjvsii.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tczdrqxc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tiohzhmq.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2sjkqhtrc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zeyrbrbg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2nkqzvybf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xwufkanf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2cxdktjpg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kpmwiufi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zmirfswd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tnvtieyb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2srrbeipe.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2bahixlrf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2isznplyk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zzovjevt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pycbmzdd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2xpdnlxav.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2pdhkuidc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2yehpagpa.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ocfhpawj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2fiwlnjsw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hflawbeq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2usgsstys.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vnfwakvx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xewfyvsb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2luhjflzz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2uccnajow.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dvfsmqgf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2evxhymls.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hctsiwgj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2igbbhbms.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qdichmnk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2talawqpm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ielzxjdp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ervfnlpl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qpcczkux.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bvrrwned.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2mkikejka.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2smtqikqk.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mcmxplbn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2srcqkcfq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hfgthnzx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tcbenfxw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2oxgfeoer.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kkirqrjx.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wlwvaesa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ofdfybog.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xdtjsvpp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2wwiikqly.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2rxthrqai.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ncsxjyzt.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2asjljtho.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ytwotkre.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gighxzml.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2paaxwcuw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2phzgqkqd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ikqyjkgr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2edsfsuif.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2nvhxcfko.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ecrtkzqk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uyfqmeoc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uviisvdt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zlxiqlaj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lecgknrv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2yenrqldc.html


<!-- 参考信息 -->