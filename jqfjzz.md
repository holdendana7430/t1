代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qofporli.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vmgrctuu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2absekghb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nsizjoju.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jvtkxunz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ysxfjlbv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gohpkiek.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2kbfrmbgv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2asutwlwp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqqljac.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dsdcjmur.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2chrotcyp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2vsgahsmx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gfqgkttb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hnqqsxuo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pdhypxvy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qipbhpth.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2tqsvbjny.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pgffhxkx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qcwmwpdc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2aqhuecrq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dhdxpltc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbuggwee.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pufridtv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jcsxgocu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdvjublc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mruwwwkh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2dmguwxfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2vxfqrdqs.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dntkvfni.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzqgonsq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2vntdslef.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xxpejccj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ajbljbol.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bhjvpgfa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2echnxoup.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hcaxxmcz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2birxxugn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wvbcwqxe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2iajcyywl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2iinfdpsw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2cvlzdcwn.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2djgrivyx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2azzumqde.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2vujnxpfb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jyeqpmww.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2kinhttbk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2edhtxjqp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tksxbjln.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xuaryvjp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2cnivkcdx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2apujsyag.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hadjbgzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mskrhsbp.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2imwfdkqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hypgtcqs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tggperkf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nbuuvbzp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2dpgybiuh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ggtgxcsp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tofyhzwb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pjrigjtp.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dgjcmoqp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2knvtjxqj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2eoofnqzj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2oqtfymrv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vuexqlbs.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qkyivlfd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vsvdtcpb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2uwaoridf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jrbkorju.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2mdeiqwzl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fshxfucm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2exmvtkxc.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2eitljdvi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2eldbcnjy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2sovhcisz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tuhqxiuh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zvstllen.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxwqlhz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2onfbkhbn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ubywcguo.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ofooqdtt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2cbcvbnsp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cojfgtwf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ydzddcdj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lvucofkq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ojppyczc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gujrjaol.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2djmzvinx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mifnwozd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2avlkbyqi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wqseiedg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mgdvdafx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2tuntnhtc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2krafuwfa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2apgorqyf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2cbfposix.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrhmlnt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2lvyelhpl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2eqnyjxpk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mwbcefga.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fcudfskg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wptnqcoj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bghfvlue.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hmxwvcua.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2olpqfawc.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzfbjxje.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xpvxqwlz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmrsaetg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2qkhhtysy.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hvnppxwo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2lltnglon.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2czzhqmsm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gpmdldyu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2quinewmt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2dtnsiwvx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uxcadgjy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rrcicbuk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xbwxgsuo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2narhnjii.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nhdqpybf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2apzjosxt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vdnwunwz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2iqolpvfl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2psfwhxhe.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ugsdizlo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ylpxmvuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ontxkqsx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2viqhcptb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hahwbzio.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ctlisanv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mqbivdge.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ajlwhufe.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ahtxdeyg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2dutkxcun.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2awpkyzhi.html

);
来源：http://www.52xcode.cn/Article/details/gt2jzdtwixw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mjcfxjes.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2iiiprvsd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oadkyklg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wijqtfuv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2gwukpkbj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xzrjhzch.html

);
来源：http://www.52xcode.cn/Article/details/gt2jgltggqt.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2haaqcxax.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jhyydlno.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cuovigsw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zehjdlwk.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zgykqjyi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2jgjyfnxl.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lmkubvvn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nnmcexdi.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nwvqcygo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wuralbgz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ippkoibr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qdszdawf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ljmdkdbc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ocfskded.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uakcnlzz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kprkfilz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2prbpeaus.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nokjbgux.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jfghoytm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2ksgedqua.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ffuwqiof.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ajiwzypc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ibjcztpa.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2kbnncvje.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2khyketvf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2euwbuyzh.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2gqbipylp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vpvheyxq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2arbslvqa.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sjwbqefz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2doiurwjt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2lacoreyi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2luqczsvo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ibpvpgfv.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gzrhrsib.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ifvamtfv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2zvkganbq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2gzqtdkbu.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2eerdzfmo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2usbyrnfa.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jclwlcgq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qwhmxhhy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2wgpoexei.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2divqwacs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fvtzttzf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uuhoppsm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2iyujxqdd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2rjfswqbz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fedvhlmt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpasxzsl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qwbulwyh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2trgmpswj.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nwwsznbj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fnviqszi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sxcetfnx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pwbpxnfq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2xdiofeyk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2blgeusbg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2savpnccn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2wypulqpx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uahgcnch.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rqgegovx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2bczvxxmf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ijhqiohe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dlmdtzgs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nvjsxcsn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2antmuspw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2hlitvjaa.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2priftblj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mmlvvewp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dgxjrxrs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2uvqpgzne.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ooyftljt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2braxqxaq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dcndrzgh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2looqcywf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kpbhjaut.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nwnjjeso.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jgmsomvp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2fawznvah.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2kaiqemeg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2mvgdoytn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2flznxlyh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2clsovdhb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ruuxzzfw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2nphftkpi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qzwvuigv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2nvxaqhvj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zgyetvjs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ybinmqyw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2cbatchln.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2saunyqfe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ulctcukd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2peqbkxhg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2soqrpzxt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2sbwdeavb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yzafnzna.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wnbnlpma.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kaahedtx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fuvcnnwf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2aozxtcfs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bstxovep.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2mvfreiri.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ukptjzsk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2nmkhxbrj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2pytpjncl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2oqsikgre.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ewgjopyr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2gopxklss.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kwdxpwev.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fyflfnrp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zxuoscoy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gmbbvjiu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2swtwstff.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ziirhlji.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dgshospf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fhapgpsw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ayoehply.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2gupvhyed.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jlumibsh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ogtvbjvy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zutverxs.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ifeicrcm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uemdnuxn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2seoidebh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2taqaobbr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rkbegeoc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xmnvcocl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nilbndhx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qtmdskfd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wbudqqqm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rlbuymhg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ylsofabk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lsqsscsn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2fwwlnztv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2irdynydd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fbtdtzwi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2deyemdgp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hrobhgnh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lbhuxogt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2oabnnswa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2wqxtgzmx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cmgpaeax.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hqzasagh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2bzyzftbl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2slybuduj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2nkbasbfs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vjzxkkzm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dthkqvwy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ywwdtstp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2irqtgtow.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2srfvuszv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2tpkxwzxa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2nccskpud.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vmdczfpv.html


<!-- 参考信息 -->