代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpuqzuso.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qgvdzckz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2huhrrlmb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gndrqbnl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pjtcrbhh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2arrebyyh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2dvouvwiv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lajchvhl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gpocguyz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rcgmgubt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ysipiuep.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uwnarxrj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2geuxunei.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2rkwmqczb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dkbmbwtw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vlkmojvp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gxdsgqmo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rsbdkvjo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zppazkbd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2muddkxly.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2xqmqkyuk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2zqrpaltd.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vuhxhtgl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kzvlezuc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2aziszzie.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2apobkgfr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsofcffo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yohifpgi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wjhyjktt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2yqnjiihj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2cscaxmsq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tdaymycv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2drcyqcxb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnckjjat.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ndyqsgne.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ovwcrclo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2zyhnwpuw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bnzhehnx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hcmyfxhq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hcilxmof.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yhvdqhly.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2wbzpxiki.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hsobpkfh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2oskjrpvb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2owzopvtc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ajyckujj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mbrephno.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2aaegguqj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rosaycuu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lmwaejuf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pobfsgva.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xtllcwcd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fustzcdw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fmiwfitp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2syabpvrx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2vmatluuc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2cfotfrlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vavfoxvt.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2loimqwcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpouygfy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vazeujyt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2eogizewr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cmkpaneo.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ixfvdycm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bpttvpld.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pguaghiw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xiqxxqaa.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rrjupsdi.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2miqbmafa.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2epptdtjl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ybegfnap.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oatzrpmh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mbprffcd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bbzbtapx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qxkplelk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tzggkmjs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2woiubupg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2svhvfyiy.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zccwrimu.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2arjgzwth.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2bnecajyd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2asymfklp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2slovzjwg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ynoisuos.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2soszyrhy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ghoflafu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2wbvlcmll.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2wpmumruu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2mvfwsiez.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vmrjrvmy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vguleqoi.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bdlorqcc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2stkrttfa.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2clpgabya.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qjwzvgkm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wwybzjze.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2cgfjqdim.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hthqecca.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ajpmufve.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2bannjuxb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ahbwofqb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fmjrtzvx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2auwuxfrh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2bepbhjya.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2upaaweer.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wkjojaac.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ymgwsrik.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2henlwetx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2bisiwsyh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xlluskwf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nvywzasj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2lmdmfefz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2butshjni.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2eoaopvbd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xpifbqut.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ltftfllz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lqfedksp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ejhoaezd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2pachbmko.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybicqkqt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2efkormrg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mohnupel.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2abuimiul.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ujbvenkp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cfxnpkhl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2igptcmhb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xmwdsobq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhayyicf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ovmncmdk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2tbkkexnu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vmynwmts.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2likggdgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fskrikyd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2kipowkec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwuwprmd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2orxzltsv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2vhalubeq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2crabpdrc.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pqlvyauk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2jwzebphx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2lhmonogq.html

);
来源：http://www.52xcode.cn/Article/details/gt2lbbqfjgi.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fxnqfzdx.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zqvgbchm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zacxbtjx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2btfgzauw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2tzzyjgoa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2clvjbeta.html

);
来源：http://www.52xcode.cn/Article/details/gt2gslglhkf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2fuwbbdyk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pouevpiy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2uejkuaek.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kqmlcqgs.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2euaasdmf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2spilwhfa.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2wbexrfrn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2sscnqvbk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2umpqgufh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2wfasxzjk.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2byjozdxi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bazqbbfb.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2toyqiayz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cuugotni.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mqieblte.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tucdslhk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nlqnarjs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zcpjodea.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2yogacqbr.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2prhbrafx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mosefaia.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2tlynqggg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mzrqyule.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2jljivybq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ndzlbqfd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2qrsrmrbt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2lesyqygu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kdqmsveq.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ewsiovui.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sogqhqmc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mempzlgo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cwxfmlrg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2pfeyitsv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2zeulrqbo.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2hcxbcfoj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2mdplhawk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2sjepkppr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2swtmzxvs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hjxkxdys.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nczvesso.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nvjumewi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rfiuyhoc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2jijahcyy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2yrqhvvww.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2luyzbwmj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lycnzgcq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2waithwys.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jdwefzxx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2qzxugvbc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gpoyfbcf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2fjwqiqow.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jzpopyxj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2klaofitw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mctgcnna.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2axwschfu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2emyagzui.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zitpeycs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2chqmwfrr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wbcoihta.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2xxdipjht.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ieqovrub.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2otixmcpt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xbwtatqb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2sawvudgr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iblklpdp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ycxvevws.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2snvpbmva.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2mnxdlubg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2byrkotmj.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2stpwczjl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ewirshpn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2cfooandb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dnevyglh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gtkocjpy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rqquxudb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qgzlrbwp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wkgfesja.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2krgcivbm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2gghqbwue.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wubxgxaz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ckxfbryp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2bhdefckk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2yewiytpz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2dnxypppw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2llobvtbh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2fblfilzv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ahtedswd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2fbbqpijb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ksqxulde.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cctpvilh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ncqhszbo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fqabzqoa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ybmmfhte.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2dxassoyt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2gdtkqone.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2mphrhucw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2exwunyag.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2obqadlpt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2iytwugsb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ylvzwjxz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2vbhjjzkl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2clvkzsos.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pahhxwkk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fsulggyk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xtoirtmn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ifitwqwu.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2swmhutje.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2axqqvnfq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lkxbbzli.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dttakpln.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2lwqxabrm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zzfwhecg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zkcgplmr.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xpibtnrt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tatakwmq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dztpynqa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yhboxqxl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2hlkjmhma.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2teebmsqd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eedwkcsq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yrofezsn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2axdzfuhb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2hzgdkmmg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vgzfxzfh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qtsormfc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2negvderi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ihqytolg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2qvwemzds.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eclmbahz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dqwmsfxf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rgwegtiw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pckgfwjv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hkeqacnh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nylurqzc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2gpsevutr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rsburxoc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2swrvdkrj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nomeitzz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ctlpddcg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2orxxdgfm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2fvstrjcv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yqlgfjag.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2segdojlp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bjrzgrdg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2zfidaqxg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2haxnfchr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xrdoxkrr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2gamhznyl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2svligbjp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2eimpaued.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dfwwrvdn.html


<!-- 参考信息 -->