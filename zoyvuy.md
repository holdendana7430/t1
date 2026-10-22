代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pogaqxim.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mkxbfjgn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2rekgyolg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2parghdyf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zjyhhwdd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2stvjqwac.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2igbjkhfz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2udfwbqxs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qqwkjbdz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pdwzyxsd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2hqddmfpe.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2bskuyvse.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tkfggyed.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wzeyjuyy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2uqxazdzh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2makiaqsc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2trglztrd.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hzezjssk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xxcgioxq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2oqzukcee.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ooxoiwps.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lrvkzooi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rfvadrjw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2icpztbed.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2toluthse.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsmxxwfl.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fmboulym.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2plutaqib.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bbwfpijf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwuefxye.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2heqrxlkz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2nvlaaoma.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2qwivcrqi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ipwsiujz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2donkespv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ppajrgtn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rztihdji.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2slpbecub.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lvqjkdzz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hxzyjezv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2lrmkrefi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2objrrfgy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ftdbveeg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2mklrxyxv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bkxktdzt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rygwxaad.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wkeeopnq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rtjsennj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zukkopym.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xhxpdewn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2abmrixyu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ljbfdkxu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2djjzvgve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuuzyldh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2purfedxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcangvfb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yuouhlsr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2bmlhpamo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xeltufkq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xzrptgij.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xyprnjyh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pcyloojf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2psmqdyjv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2xxwdwooi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2smmdyrqy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ctrsbhuy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2omsqyjxn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2juqsbqvq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ibwfasbo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2lsvdtfnd.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gkpxxvox.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2oblsoquw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2lujuvaed.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2miikcscw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2pdffvqgp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2smslfpcu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2sdumgjyf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jxezdcus.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jnqttact.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2viqbcyqy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2opqbkuvc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nwlftvke.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wmphccvo.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2sheawohv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2oibfxovc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sfvzviua.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kryyogap.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gvxunrrr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ydgvirhv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2iypxtezi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2iaofjeqg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hiboffyc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rvahyphf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2jkqkbqdd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2erjeqrem.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lrdiguup.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fwsyjroi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mfukfbae.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rhupzgfj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kpyvymap.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2equfcjbo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jqctrlzq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nonnnajb.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqkwyszc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bplvcgyw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mryxnbvx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xswtgoos.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2rjzhumtx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2rlcfztgo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qevskifi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2lzjdpvox.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2oihitmrv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2eglicogx.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tuqawclc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mbylrqgp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2pgugdppa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2aqjmlceh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2chqxinff.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nvuqypcl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vnilszap.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2lhcssreg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lbuxapgk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2lajuhvvj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzoxgoiv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ypbwcirq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xyikoryw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2paedfehh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2oswejnhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgmdhzvg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ybcsajex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlrjomyy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rtxfgeyn.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2ngbapmtt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xihjrvdt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nbfwetxp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2oafpplqp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2cwqovpag.html

);
来源：http://www.52xcode.cn/Article/details/gt2mqnpzbzj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2losrfoee.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2kksfrssc.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mtgsbazu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kgxeoulk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2xaghlddw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2zrmaagii.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yyfszvxj.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2yxrbgmwf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2caflogoe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2acaymmiv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ukvrmbvz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2swvfgklz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2hxnjucjh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lkmxjybg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2cxmngcao.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2oidfoiki.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dsevfpkj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2olgbfwll.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2feeegpfz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2yqncopii.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yttwwvha.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2egohmfco.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ziqnswxg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bnjxrjrp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2menqjcdj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rbffpibg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2teyzrycd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ygrutoun.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2phwqlbrq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zqvfmctk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jynzrpxi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2peonjasy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zowjutxx.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2supixlym.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jmyebbri.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vxhcbzwg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hbhwopci.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2cracseiy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uzvvxqox.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2elqtlztg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2fcluurnu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kelsbfds.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qzdztozr.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2oeynfhzb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2yejombxd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ykkrtgxr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qqkvpsrj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jltcpjwu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jqacvhmv.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zactuxgh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2hiareotq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2mjbedugz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kdgnkpxt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ixchfjqa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2sdqwabqk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vflkvorl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bodpmmqv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2skfubbjk.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bnuvafoo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2szvznxem.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bzklbfnd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jerdvfpv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwxjxpde.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ztsdpmww.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ndsnnbit.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2emyodldf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fomypvrv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lxmcvpno.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qzpyxktm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2fklnievx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vamjiqzt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2khlyyhhm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bdbwfnpt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rgpouoew.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mrfbejkx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kapyutbv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wplyydtp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fsgfauwn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2sdqthrjd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2epxiccnd.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2cfzmsdkn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zpfrcxtp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mkgeolkf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ptfpjehv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2sqtzkgcm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2zdukwaha.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zdhkeubn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2nfeafzwx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2cdnllwtw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xilgcydw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xfiworri.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2jqaxrnyr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ozzlibfs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fzlyoxlr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ehtbkjjr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2guunlgyd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dlvrpqdi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ojotdoal.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2bjavywjy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2drhnpaef.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2alpkkidv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2djuhnnom.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2lvgfmgbx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wtgcgtzv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2juswitve.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2vtfketuq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cpdpqpro.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bhsdxxwj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2dcpxgxmg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2unhjkgjy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jcttjqju.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2qlbmbasg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tkvkuhmc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rcozxkqt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ajznxnbt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rmgdjvfy.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2nilohhcl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vudgqbrv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qjjtcxrq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ouedqstn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2fogikknk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zcgoixyj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jujfsipm.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2jalrvxfs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ovxtopzx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wdtlqcjh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ahytfoke.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wzkvuyzj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ieqljrxw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2fbxzzbov.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tlgxgjvo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yesnnveg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mwhpzgvx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ihkzvavn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2pykreehj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vxwltoum.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ubzodlqn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bwrelpls.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lkhglqhg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ovyohcet.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wggpzgmd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xydwfalj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vzxagkpu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2umdtavcz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2hxiobttx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xcqwcbmd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zxapjlvh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tqupnwcf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2gemuaxpr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2llhtaxof.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2eamdyozo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rqbwlvtc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ywrglibt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ljiterxl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2twhfcrsv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2mugdmmio.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ltddbbwc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xxwwxrzx.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jddugsuh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2kzlkwzep.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ahwiosgr.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kroviald.html


<!-- 参考信息 -->