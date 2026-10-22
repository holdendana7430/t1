代发 wailian999

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gxeyiqzp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gfdzkeeg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dzlruwdc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ejwbjmon.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zaqdfsqi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2haetkcds.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2wljfjnko.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hqwzmtbk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lbsiwypa.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2csapbobz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gbxzbfbt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2latmnjrh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jjawdwil.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2trozpgeg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lndkdyke.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2txrznuit.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ffurrdsb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hbncwvfs.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gfsmpttj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qeysboxj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2nejnypfg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yworffzy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rcwnooxe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uebxcrgw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2kuqrdmtb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2uwinokjt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqxdxvqa.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rhiepdqk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2wwtsyajo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2huvvaiox.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fmwdcttl.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zjtvfxwi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hkpxicyd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2iajbvbch.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fkxnlijg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2djusxzee.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2uepqnoen.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hepkdtkd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pdrlrypl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dvvcvhfw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2utviciwb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zxkvuvsv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jonyczww.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2sqxihqgt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tufztpbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrnejbli.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2oimfbvhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbkfuppe.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rxakfnii.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kewnpdmd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dwkmccyx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2orygmmqq.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gsanqsti.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kbyghjyw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2bkqholqi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2yyaqpqjm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2exhkoizn.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2saajsdia.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2leqbrudn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ubhmrmbd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gvrxjzuh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2uoiwaled.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uoprfsrd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2imjmyqac.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wygjwikn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vtfqlxge.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fzhsszpd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2eptmaeoq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2axkdnidf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qogunkqp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vdyeqexk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lffzdwad.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2syepadwr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tngjawrl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jvgebvft.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2iszdclki.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2pmneijfz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pomiykad.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pcuablzp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wqmrtqzc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oyoxhwzq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ypfepvlg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2pexserse.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uuxamnaq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lldzjzek.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kaljdujn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bqjlzwwi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2batodcuf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qwosgdhj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rbsmubbl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfbvxzrq.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2yfjcdrlk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2fkzduend.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ubyrxepz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2olmzktds.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucruyslj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2amadgogq.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2nqvkunzh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2txjlsrol.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2yocckzcv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pajzzssj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwnvkpcs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2wypiebfj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jzhtkjzm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2qjoiltgg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2agohrqwl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kthnpult.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcsfbbfz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2biadirlr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pwcyvqpg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fdvqncki.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2akncaybq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2lpairbhg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mroduafi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2fgkjlgcm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wdenrxwd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2pdgnqxln.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ldnpnqvn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2xthzhzhz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2akbrmdim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efnaqfiz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2koriggqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efgdfefb.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2guschhfw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2abtedtpn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2spgekqta.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hjbvsppq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wmtbqvro.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2eshxgryw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ymuncppu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2eoqlckkn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2mogmsrek.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hlzcvyhr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2minrfsky.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2plegrvsd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2rhubpfiy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2byexoqyg.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ifxfpdlo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wpgbcyev.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ysxazejo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mekqwyts.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2eytxabnf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2gjpeyrzs.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nyuvabcn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2udkougit.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2vpykacbn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hjwrevdm.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2lskqnayl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vhaaiyfl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xxswxkbk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yvnucaad.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2gjgkpktp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rdvexyed.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2agnczkok.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2obhsshqw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2xclhjeoe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2royyxvek.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zrrulqgi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2dybbdgkg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bzoailiw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2gmwgmkwa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cwkklsja.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2lppnbjlj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2skbsscdp.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zjjdrvgd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zhirikay.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cmkrsgiv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2dylgaujm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2edlxnijf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2sctbwpmc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tydauqgm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2labjmbkg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yevdrqrc.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2utdyxibq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xkaetjkl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vinwgtpr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2rgkcrvyc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ledhzwop.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gglytasi.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ucqbxcsa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2uctqidil.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2plltexjf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2keotdlwq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2etdeaaiz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2wygawbxp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xdraozdh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2orbvsyyv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2klwcrlwc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zndoqqna.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vhdchzld.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eejbrmbq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yzkhdldd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rfeqygpg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2sbkafxci.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zaewwxsz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2paznvkfv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2uepdhupv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rzrjiotb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aubhlwot.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hyuqwqvs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ggrbbijp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2jfcyftip.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2juyrshes.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jckmsgud.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hbwdlzsc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cwbqszmo.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2pqzgkzad.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hhffptvz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2chgzjewv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2txclqxfm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2aojelfjn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zeaadvaf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2dfgfxeuw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kdvususg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2avljomrd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kemalzis.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2lglpqwdo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rogmitug.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2sxejneob.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hsderhzx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yaygjyxy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2wmcugbmp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ukrovtml.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rgdpotee.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2iykspxai.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bidfnycb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rsdesdlf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gkisqzrj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vpqrrmvc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rrxkxsbw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2uvhhzrgc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pvtreuvr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xtrwrpjc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2nslukdqy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xrllcodd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bleewnjp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ltorpvhj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2sygifitk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2gwxiqqhj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rdhdqmtb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fkzuxjea.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2mvtbguhd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qljcwjdp.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2dblfimeh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2kfyyquhn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dlomrnyj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hiscaowv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pmvrgfrs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2aysiwffe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ydnejtzi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qwfosrhp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2keslvzji.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dhfswvub.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zrtbfaka.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nmrzxkji.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2ssitsfxl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rbxtjlik.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2oxbrrhvl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xssopogj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nrfymojj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nwxvqxpf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2wiltkyni.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qevxxzcs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tmybdhpo.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2kwqksnlw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nlnqurun.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2tobdvkah.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ceebkwac.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2oeeflgsm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tgdrrxif.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2khlgmfzh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jdgtvzkv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ynxynegi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2iookqfbh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ukkuruhj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2sdmazckp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2abnjgmzp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jzzxonxi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nkubtcfg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zozjmkbb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mpmezzkw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2veiyyqiw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nabtstkk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qppjjjtw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2rvmcwjri.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rqupefzf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jiirwvnb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2odqflqef.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eyekgzsa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2txptitdt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2atjuvkix.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qdmtzpsw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nqzrmuor.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uixfndio.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dbstarnx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2liozuqza.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2fxgwpfey.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pjfhsqun.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2riyqaopp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2eumsujwm.html


<!-- 参考信息 -->