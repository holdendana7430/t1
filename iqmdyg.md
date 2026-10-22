代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xyjiudoc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2oqffxtll.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qevymbgv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2sfnrhwvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olrlrqzp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gkvyqfoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyyyhknf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2rquzrrxx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wdqgrxnd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wywgmsxb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2anbayjae.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2abherdbe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tybrbsar.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2beyegqkx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ooumwawd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wvqkvwmi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gidefmcd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dncinvlx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kqvbrlij.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eheygjii.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dlkestlg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2gwxetywp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rsjeyysq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2cekxodph.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mxxlwpoy.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ormevmcs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rmaghele.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2fuzotoma.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2scwhswye.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cootzemd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ismiqusx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qlrjbrds.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zcjuupfq.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqqusbz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fqxttish.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fmhaogog.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pyyyofur.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xyjvzbgk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2teiearxj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ggfggejd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xyfvxpqw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tiucvpfm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2emsyyscj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kudmnyxt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pjxqhvcf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2iiqmkreq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2dypthvvf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2igqnxmtf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2imxafgux.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mbgcasfk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oonuqcvv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2iauisloa.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vniccvsp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qvrbbirs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2earkkarj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hviluwua.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2cnecnkkl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hnmarrlt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2pdmuhicd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2zmzlhctv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hzkkmqsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxoqthae.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjtloumh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmydtccq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mxyzvojb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2enfsvtij.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2sbicinvd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2osgmpwrm.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wglcggad.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2cmmobufm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2takunkpk.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2czlhrpdj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ujesungn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wjimhioh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2njoknuwh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkzhhrbq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fqfeiwts.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wvbdwdpk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hyiiobkh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xydudhad.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aoijvfay.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2llentcsm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lzgtebqq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dhntlzcc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2illcfpgi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hwjopitn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mnhbkirk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kwgulcry.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2amkkfyyu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ymntuopw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2nwdrxsye.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2uzadhujg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2nmbudwwz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2psfunafw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bljefawg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tsmniarz.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tnbxdgxi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ccgvsqyl.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jgysxyoh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hcikrpjn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2phlhsqkv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wkxvjsaf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ribhnonh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hxywuxnv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xwzjccjq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ffuoyfqw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ckmzyvnx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gypybmdb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2jgrofvkb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2cwyauarr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2xtpwzwzw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2roqbuyjd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2pwaswcsu.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2haswdfdy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cadqnvqj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwejvnmr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2oxxgnioj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnrkwwuf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xzghpwyl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2msckvdyj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2rpqkyoeh.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2btxlnfgl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xjxzcsnw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgrtvxju.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2dqmozgcz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2iskjomgy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vuxeaqkf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pzwvexpv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2hahvlrrg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ptdjynge.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ypdvudof.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zqfvvvgu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2otfonkxh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vacldaic.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2miabxfhq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2gmkimkai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csyrnlmr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2flpfuauw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opjyhohu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2sctqvngc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fowgxkbl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ztgfkphz.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wbzpxpdc.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mvepimai.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2hfsicnwv.html

);
来源：http://www.52xcode.cn/Article/details/gt2pmfnlxyv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2rancfrvh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nndexryq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2oedezcai.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wqmntzzi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2uirlhtqr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2wqstyqic.html

);
来源：http://www.52xcode.cn/Article/details/gt2izfhtmbf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2rvpqpjye.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2awxwfkdi.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2pugnzayt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mcvchapj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fvzpusex.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2qkhzeedq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fkpmttti.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uvdonezv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2lbhditff.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2zetvvsec.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lsnpsumo.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qfrqzawf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2vvhmuvbt.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2vhqkhbey.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ffdgleax.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2toomqvmj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2rffcukul.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dgkdyjan.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2fqhcehrd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2esqotucy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wlydtnea.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2heasmpus.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mqrkgqgl.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2mxwphdnm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2uxnjpzqd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2imzbeyvi.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2uabrtlmh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2esnshtfx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2osvobhrg.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dkscbcln.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2jglfsrvg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2utrdbuls.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ctbbiumt.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2qyrrtjfr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2wevjmkdu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ahbsixqt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2crkyajim.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2zbrjyeoo.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2ykcsnuij.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2dajvxdqc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2oslqqrsg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hbugcikc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2agallqlv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2wwjtlyyw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sckhwphd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uyzlfjne.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2yjfssybm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2drsexqnu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hdyfnfux.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gnilaavc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sivyoibz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bwtpbirw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2jdjmblqy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ehfmzdnu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cshnluxv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2levaiwuf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2uxdutgdg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2oapmtvvq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rndsfxwm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2qmuvqdbu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzxoisfw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xzzbbvki.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2hbgmfxeo.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2owrziqny.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2sboxeyjt.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lxnwkdid.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ykumtpck.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kjpgdlom.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kswbxevy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2pkfespgt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2brejmziv.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hdezqmec.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dmqkwvid.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jekmvgqf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2loiarkhf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cwpiddbj.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gycwzljt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2znktztia.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2bzyiddfj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2hogbhniw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2qovumnwu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xrcefstg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2esfeswln.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mmppvwig.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dwhrvzsg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2vpzgpecw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2odtfkqro.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2huwsagwb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2uznbjlbb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2oenkssiz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qbxwyfxi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xsjlvfjv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2elxomknv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2vuguheef.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2royyxwcx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dpgtfdum.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cfmdbxwn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ddnmowqg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2tatwwqcw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sxeuwhdc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jltspuej.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2vprhofco.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2lcmhjcja.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ggpcrjql.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2cafxxtuu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dpelbcco.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2borbafgw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kzgtutin.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2imlajvnt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ehdfuvzs.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rzthcutj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mrwtkytm.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mhjxqakg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rkztoyhn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vfhibpcg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tfqlxstl.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kscocxzf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ryfeymsk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2skrttrob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aybyxewp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ygmbbwvn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kbskpgkv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2oumaxgek.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jyvpxvnh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2priyfask.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2avgizrfz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uvwamxmk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uupwtnof.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lwqheaey.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2usysmxug.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bhlrdgxu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2hbyxqipu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sxjzjlnc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2yqjzoask.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bhxcazou.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xzkfzyon.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qahbrreq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2fdprwsqk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ciyebgxy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2wttqdgmm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wjilrasu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hmfodnvw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kbsgjztz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2womcndrl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qhjxplss.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ihvphqtv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lqybmoda.html


<!-- 参考信息 -->