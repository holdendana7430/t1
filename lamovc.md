代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lynevjip.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mmjtiiol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpqvazic.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2xvhqaulm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zxndfecc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mndiphuf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2zrephsxv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qdugiazo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cbyfcrbo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2hrkwuaqy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hoeljlyq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jnwfuhmp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2hyuzcefu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2efxlrkza.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rxphiiof.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jhmheqal.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2okmbimpc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cknsavpe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wxizfpbn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bcmahkvd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2kjxewlie.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2reamzweg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2isgwwpdn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bectpmni.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2juooelml.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ihtsukrn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddxhyoxr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lualmeik.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ycdoobqe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dhhpmfew.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2akmalrpb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jomgkgud.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2oatgjtwh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvokedhg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhkpoevt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gawwabkw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bwduqxwf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2pehvsibx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbhnyxfs.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jzedhact.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mntclzbo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2raahqzen.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ilmorabg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jddcziiq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wghwnkpr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ebdoegio.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mauykohk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2cxuevshb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2haipkrya.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2elglbavz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wuctsaaa.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2akenwrxi.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kzwlezht.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tfdjlksw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2inkrbbpe.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2izhpcaie.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2bzbytfpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yombpcji.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ajklukhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkajrwfc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eutjndkm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2hcnqkkaf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hbncydis.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qlpxlbbm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2daajxxtg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pzvxqnae.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2izttdkdh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pneeijoi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2huashxhb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2rrzmdgxo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zotlcsxz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xmmleyjv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ftlkqqem.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rhxasgnl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fnjqqcgb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2msxbtvcv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2eyylrbkt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kjdnlhie.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aqzrjcvn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jzppnepl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2wmkvtwty.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pcfgsjya.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ouaqcwup.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vdycxvja.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ujrkbdzi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2imufpkef.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ifkwfuwu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2eixgofqg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2gnjypjis.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nynvpnmo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2eqsedpkt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ivdjfrfm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jxigpzdk.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2xiavrixs.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2uspnbmms.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2newoepbc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2yeujelth.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2anbfrkrf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lrtrzlrb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2xyozrpvh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xhgwjdsr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2sfvbufey.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hbajfore.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ozkmzuib.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2kbjhjutr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ovvgqjpx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xeamtars.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xccryhth.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2rsvgavkm.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ntkilrsj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dphdyquq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2cdjklsyg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2yudhlbbe.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2jttmizau.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2thmgtrhd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2unoyssll.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cqnkzwrf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sdwrhozp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mrmzxhuo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2apzntjii.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2rqwhrcea.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gytclnho.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2gqtixwtk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2dpgogypp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2ftflfxjh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exknefkm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2oppznrmk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nniqsqtp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jyimpksf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2nsclxvlp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2eqoeiwrw.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2oiqyykdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccxabunz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ynwigtaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juhyvfhe.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2dgdzqton.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2difazbsl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hgmlwfcs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wqaucpvc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2olqrytuo.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2uwdqdmsz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kzvfdrbt.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2fwfdcdvz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2scyjfrdx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lyomppgl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2udjscvse.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2mjuzfjzo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fkhcirdx.html

);
来源：http://www.52xcode.cn/Article/details/gt2ifimoajf.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2aydjulji.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2nrhxnrtv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iulircwn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2uhwrwllr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2datgsczc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2splscadm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2nwtkxpps.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zdcqsdhq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2gtqxdbpc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fvtvbkle.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2khmeittj.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2yjkaktjn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ydxwoogg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2aknkydja.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2qstlwwss.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xikgimof.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fmvzowzo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2uakyusrp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vzsaqkew.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2nzzplmkn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jluefuxz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gjdqlyeh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lqermoue.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xmkfgruu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mhaudqpf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2tfyyjdlj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2jmeexzsw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2asaqecro.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rmbyicmv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fxewhkns.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2sgvpcjjp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jtwfjklo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qlnvuqjt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rwlwsrqq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qzqeriba.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hbcxjpye.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mkiwkgrb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2atgbowhd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2rokbwfpl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qiyrvexg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2lmgqphax.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2dcjcdpis.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jsangthp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2vndneauu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ctlzlahw.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nyngluuo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xdhsmbyp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rzexxgeh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fqwsvsuf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fwdzyssp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2demsgnkr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vmavvibc.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2lshqvnec.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hudkvtro.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2oprsfgvq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vtoigrng.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2brwzutxi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bkrxxjnj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ydfvicfo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jlqvzskh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2axdujkeg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iqjipmlh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bkyltyjy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lbjftkdr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2uuxblryb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ubmxtanb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hfenharf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2sqqqiatc.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lmaqbcij.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2faiuhzem.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2poenikbx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mupukpzb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rvamtdry.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vpxbfsvq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lnwvsrhz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tdfcycii.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ngmbduod.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2djtwcmcb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ggjtbbdt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xtwrnxpf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xilevsfm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2raklgtbf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nvtejtow.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2umnkjmrg.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2axzhdaqw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2oaecrmmc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xitaehtk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mwuthiip.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2boomarla.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2uvflopik.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rtxwfyvc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjwxtgga.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2glbbdwpw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2xbrkiwse.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2irswqhwp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ndtnrfpl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2powlgxju.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xmpvtkvk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2iacptars.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2yjskskje.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2kyjecuyg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2debmmzcz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xtsxikwq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2roscspvl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ocsznffa.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qqugpivb.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2bxrlfrek.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ezzfzpze.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ptsldpvc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dbswniqa.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kmgqprau.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tupdqkqq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ekaarjpi.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dibpjmwf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nsxzdokq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2llwjntqu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iqqonfam.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ayziyntl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2eniiuqsp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqnrjool.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pxglxfmu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sfxppwbv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nqbgbflj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hncvgdta.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dkxfychu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zlpraygo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pqwmojeh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ubwhzlcf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2delvdhii.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gfjqtehm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2afwkosnx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ytddlsnm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ithgznhc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bbqsoepz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lmklhlkv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qaxhndxs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vdxytrlo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mzuffrmg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dkvwmrbf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2csfdqhvk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2tbkwgsyo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qiwxmdpu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jaghhlrw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dxkrprho.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ilezvmnq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2yqwadnce.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2szjqvdab.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2elcsjicv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ftsstyba.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2gujuvwew.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zjvkjsgm.html


<!-- 参考信息 -->