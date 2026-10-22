代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kggtwcxe.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2otptitxt.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ecrqnljx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2exoglcrs.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bmmthdcg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nrbhnidt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2egorooqa.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2irnxwecu.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zxpluknc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2npqbtppd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hexameoa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zdpozqay.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2fhxhlytc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2uteqrbra.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2esenqvdd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lvyxljbx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2rgmjcjkp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ndbcnabh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2enoajxge.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ozrlrypn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qdvhaybe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bdpqekmu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2fnvdqnkz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2pijgqymj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jqwxiniu.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytxxuqlo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bijypnbe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bqnlhkpx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rgjkhsfh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fvqgqshg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rabwjlfk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2yullzjde.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2osawbjjm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ezxskfwo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yjivjlfe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pszkwfbh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2frupctxk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bwlckfqj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uontipoq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zwefxuef.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qdrcfvta.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rdouvyog.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2opkjwgws.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aztgfnqg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2urgovups.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2oblccwul.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qxhjylgo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ptmxxvwg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2sdftfgyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwpoyohx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2mibxgkzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjeycrdt.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2axlyxczi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bgwnpkmj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vlcjijvk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lezgupoi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dhrdfpkf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2gsdnxqgi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cpndaoyq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ennxnjwn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dmmngdme.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ljgvvnad.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jzlzuapq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2szpaythw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2nkkjqvze.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wnwstrtz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zjvwuisy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xbsdspdy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hfaaunvy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2galnpfvu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2prehiuio.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dupbkbrp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vavhwoem.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nyrdoxbe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jbbsmots.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zsoyaaun.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ryfhthth.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2tmbwztsc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2trkvcjyc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bkfupofs.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rmuiwjdk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xmjudtwv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xybibolo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cppqigca.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yndpblgt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zkgarthv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wklrmaqm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2oxkfyhzv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qufmkqbk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2gujufnjh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ytdhvsvt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tpllzpii.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvrugxp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2jbtrqjud.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ciodexly.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mpffstry.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2aylyqxkb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2yxabzedd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xxacgxgp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2eoyqqgfm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2kdsxcxne.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2deewzawm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wspudkgp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2nftleakx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2riiagsen.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jtrgafhi.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2buptsmlw.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fgjhkzwr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vjokvlie.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sxnlaezv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yvjrwlsi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxqrgfcm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2tajptroo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2rpmavhvv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2lrfjrgvn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2bvagjnqs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2eciovoit.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rrrishxv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ywnzgydq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhmbioo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fdxdipcv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2usbwyxjm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mzmjdjkt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2tzarvuov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whigfzry.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dcyvhpce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evhezzlz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xurjzxay.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fjheutcc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hnyfpvod.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2psfhyfqo.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2hritrscp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2smvrnysc.html

);
来源：http://www.52xcode.cn/Article/details/gt2systgolg.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2htxwtzdw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ayevwhcc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2iqkfxdjq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2doppijlc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2xjgtvoqf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2uitdsxxz.html

);
来源：http://www.52xcode.cn/Article/details/gt2xlhicwlq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xmjddowa.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2uovmknnw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2dpbnbxyw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2jznkpcgw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ocrexsur.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ehtitlii.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2seeymttm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vytnwjro.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ozjfdzio.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tvchbbri.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2beadnbrs.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2awnqeary.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gbeznrgg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fwlovqry.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2arblanck.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mpzcghew.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zxuzlgfn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ehebkpdb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2saxniuts.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2spvzhsay.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ldtwadqs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2bpxwrshd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nojluakq.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2eplswhko.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2gaopjvgj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lhjdymvf.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ujdmorow.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hewwxbvz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vtbeautb.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bqtnybqd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hstoewjq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2rvnzcytj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2euqdxslt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2kiioykdi.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gveuibpj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2olkzdspv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2advmltpg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lbekiwhn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gqalvjcl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2wzwnhhny.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2wlciztek.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2mwtcjffx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jwlwlhgy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2eealmhqz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lpvnmasp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hfjznkes.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2zybfmdhe.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2mqkedeoy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mdbzngfc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gaewrodv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vseejtdt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bcgecuvi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dlkrwsnu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vybvjuue.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qarclbza.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jwlksezy.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xitydtjk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2unktzuet.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qpgnugta.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2aaeflwjw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vdyiqssm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ysezkrwg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ojbbxsjf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xpjpguzo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bdqeyiqr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2utuhabcx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2raopagqk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ualxlpwh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qdtalifa.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2ctvkoxgh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2llqyjdkk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2reiqloop.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wcojrlrf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2iwdwfyho.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2asdirgxn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2acztwfrl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kcufwqyz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mjrdaqsg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gnipxafi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2akiyihkf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ohidhprc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fhejhzno.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2jnkvyqni.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ctydffhq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dcxrnjde.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qccxgaid.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2gysclskj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2uyviwgje.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lhluimnw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ppgdwqla.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wkqfvjda.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jggkqnkz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dfxwqoxt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2npiqsnkx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jggmxjow.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2aurnasgq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tlxclenu.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2drytfwfw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lfrqjfzy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rplwzoxz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ffkexqxz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2entcmloe.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pqnkpzjb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wsukymrs.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2lhtssjcc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2rhkexube.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yuvmlwsk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lplqhydd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vrybyqoq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hcitaimh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2kuffxlcg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mcrtpegm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2yslxbkbv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zeqzlenl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2xzvdicax.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hpqfuouc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ucdcohaw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hwbkpgvu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2plzdqlop.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jddvydft.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2lzxdjuvm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iihjktof.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lbndydze.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qpafqyzc.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yugwtlql.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2rycfzrkr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hetkipfa.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pxluqsom.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ntcceikm.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2hwxwvgsb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gfqyoaie.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2hmvuundl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zjfmxsfw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2klaczcqd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kppkjjqe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2irlnytak.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2kzpmbjqw.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2pokrszkd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2naxvcjeq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2wzwxhvmz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2jrfqccno.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2uydgnodd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ynruxguz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tcdqrovo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2afcvcjja.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jrmqzpun.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2hzcbbwkw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lukevngx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2xecckyzq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2viqthcxm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2brhtzasm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zuutkdsg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jhcaajxw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2foexgrlc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2atyazyut.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2lkqgtkdi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gvedxkgk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qdbzvpnm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2eaqhogyf.html


<!-- 参考信息 -->