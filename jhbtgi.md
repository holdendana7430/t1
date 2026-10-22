代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iwplswmj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qfuledgr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rqsppunw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nouhlacw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmvcqdkb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2lcmmlnvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxxtlwrc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pvjxrogb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2laacrwng.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2cmwutzxt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2uqgzqoob.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dlajahpy.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2azlqsyfg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2dpdyvfog.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2odfwmerj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2egsprkja.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nmdfayms.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ncdzptvi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2cpbazecs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nowrmmcf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2akgkxyku.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2qaqnwfkp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ycjqmsas.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2gygyrxwk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zzwcxtav.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dfrspjwx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2geayguke.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2meqyvnad.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ffuhxpap.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bzdprnkr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdtcszsv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tghrmsmp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jbxxrlws.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2byxyyoch.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ihbjrsxe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mhgwrcvj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uqzqlcei.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vadjdjrn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vssumylc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cqxiuujd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2slhpjvlm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2qztnlhqy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2swxaphhe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hmhqtkrr.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pogdirvk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2bqxtpuyo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tpcshwhy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2omkvzply.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mfodmirw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pxzgersy.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tgkutznw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2entzcipv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qxagvsgg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2parrydoi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2iopzyidf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2akcxahwd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lwjxslkz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tvcnugtd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nonfyxos.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jdnzwiqm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ojnclfes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wypighui.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fnsxbyex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2advctspr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2guuwqqoj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2bfpczgdk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xhfmzoji.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yvbrctas.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vfdzqznb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fchihmqy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rvzwcltg.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2surqotrq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rgweqihr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bpjtxvys.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qzocowva.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kiszwzyd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ridrygwz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nysgzcnr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2estrnuuq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2lsqceoww.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2whtbhkbp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wiamhldv.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xvvprrpj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ikkzmtco.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qghbmgmj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2nzkwbjuo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2papdwlqw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zurgyere.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ievjeyhx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vnukzoqg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2eecvtcnv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2pkhdzcsx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2litwoadt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rhnrmuky.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zmrkxlyh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rbnlccke.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lcuhwcop.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ggtjugvv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2fefnridm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bbyayjxm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2muyvivqm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mryhpbyq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gjvvpiyw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2kypwrxiz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mllcqvgu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rrypdzjh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2frhgksbk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2brjpqqam.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2itrjsapq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2wzdmjqse.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2thteldrr.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdevhpcf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2lzntdejs.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyejlbxq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkiuevdm.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ckeelrma.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2aawsyqqn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghttzqpm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tdijccfs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jzsresgb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2nwphgadl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yluhbzhx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zjuuvkrs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2byltrzsc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pbcpvhvl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mhlgecja.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2oihdcpgh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2frwsiuih.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zeenhyex.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2uwtazdjb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2hsjzhhjz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bqyamqky.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2sfeghmij.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2fkeoebbi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2querkbov.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fnphaboy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsleqaaf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pzueeiyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zocpxhci.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2yekhxkmv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vertiujy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2zvhqawsj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2xnrjinvs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2yoydhfmr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2akbpenrj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kpqerlmn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2uxzqdpzz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2sxehtdjn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sfjwobaq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gxsxyzdr.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2jvwwoswv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2yqbijhxs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fgucasti.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2jcayqvzu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bzvdcyea.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2eskhzccl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ymktikpz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2dffqngmb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2osilnniu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2xgaujeiw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2tbmesapl.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2rxbqiqrb.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ptwwiwau.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hrajgktz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2sgdeovwp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2kudmazfe.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2comyfsaa.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2jsdozsdr.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zvhxymjm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2juarfvvo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xyawxvci.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vimuspks.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ysjnyhlg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gdgsumfu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ljhsbaxa.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pvpquqho.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lxgjbonl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2rszuslpy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2iwysxfuy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2keezutkc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zlxmhqrx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fqjliift.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2faptbfru.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2sppizpkv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aaxutglf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yqfxrqug.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2enaiddzq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gfnhzvgl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2yyymmpiw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gzuxbwrh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oqxtyejq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2pvcjgnvv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2aweaxsfr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wydtsgmz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2pzvusvin.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2usstjfjq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2swrpqdop.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2nrckyzsb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ntbbanrn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2bocdcgyj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2inrsjpsi.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2updmatof.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qwkkdzsf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fzvsuzje.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vvnvwxpn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2iavjoymb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xheqndpj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vmqtjvfh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2azicadze.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xmoycyts.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ntbziyqa.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2agbfyupm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hmiwlymb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rydoehab.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rofinvyl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ikcmxtno.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vxygeioa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2alxeaonq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rzqhpfpy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2jvyeqlxk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ejkrlrxr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tyrctkfo.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2mkwpopvr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2tlquudup.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2vrqjqxek.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nlhckojr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2fyrnduhp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2lwmabfwd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qeefokia.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2eiigfneq.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2oaswmzgf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2iaahhxbh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2enmrxeyp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bxdtoonj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mnacushn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2orgfrbso.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mxjoeegf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2krnsyziz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2rftxxjfe.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uwkmsoao.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2torlxrft.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2tkdlijoc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qnwkoxmh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kpbiffza.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2nhhcsabn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2rezlzasn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2pwunuaur.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2owqzgdtl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2yonihoia.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dbzytjfb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2izidpgxy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ryahxpum.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gwlolqdd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2kpezgxzp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2syepmfjd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2xcbdhlml.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2orqidexw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ypygiumk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vqjvbblq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2oipqijwq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jkeievlh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2iyhiryyf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2atgytydf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wgqksnfa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ohqpfhna.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wzozlnop.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qmcltmpq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2madrypli.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2nkpbmaou.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mzdlhyau.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vftxmpog.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ummfkihl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2evamdwyn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2psbttpid.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qtzittss.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2mvfuvfay.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sxmsguwd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pcngkpzl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ziyoivjz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mrpwemek.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vjzkmqvu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bggtnlea.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lnqlgrvy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fadyhaig.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2bwvwuxuu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kbbuyyqp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ftgmtzob.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qiqptruk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2deeteauc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mamwqixp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2qujjjlsu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jnynigqf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pagciidg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zphikrpz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rdcqnjpi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2imcghxeu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jsiznuzk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2udxctsrj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2iceerofo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2fjsdofpp.html


<!-- 参考信息 -->