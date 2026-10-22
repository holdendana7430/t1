代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjtbokjj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2rndapolp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npdgmeiq.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2exonpqty.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nvbzsgsa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2zshdhriq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xjxelmyz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bykrvjbc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jrtjypxl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rkudzwwi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vytsdwkm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zoiikcjg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2epgadikg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mfvzhvux.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ffoolyie.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wmywbxyh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gpnasgrb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2azxbyhco.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lfowxhbt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ysyyodwg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2yrbkcvid.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vddeucgt.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2uitnsltn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vufuwfrn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nfmbcbbc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2dnvojqud.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ckycnrsr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jdrjnglw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2btptbbkj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2lmeqjncb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fmippzei.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mtipxatw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jkslyqcl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hcnirqam.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltwlmmre.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2eislnahj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fhuxkhpo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bwymbfrr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uznyjxkx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2satjimwy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hfcjsgng.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2gqhyaucc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqvleci.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvenpei.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kghunsde.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zfmweykk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2sgkmeiac.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zizxrcnn.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bledgmex.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2cynravoy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2aphtomqv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fbzaytcn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dqviwrvp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2abpnnbht.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2lpebngdp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ofgqfcgq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2npucyexw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtqfcfqs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2otptmvbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwktvvwk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2uqjncdvt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vpqdnlwc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2hfelilcc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gnprmbir.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nygsvsuf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2gfmrnpkm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xaytpspi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2okodcrsg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cyfnfexs.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xmvykfyh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2evllkadk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2xrtpabqk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2oxvvdgox.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2byaeonqk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cuyjqpdl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kcicomkg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kqttbvif.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ynbxzoby.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2syczuato.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bdckdxcp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2johgsuhf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ooxacloz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lvqgppfw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wumsfvwn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2rmigsauh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2umrvmsey.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2oqtaikgf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2unxlodsu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qgeaijxb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sbuxianp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sxojxiwq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2zphnqvac.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uqqzjknh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2rwrzmuqz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gpvjnzss.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ddmkrvhq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lqnaewub.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xlmablxt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zyjbexxp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jejwytny.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pvojqooy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hzrfhddx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qobzrhig.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2cylxaisc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qrewvlww.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2mkfrlhyd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rjwkxkvx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uljjvrxc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2pmfuoekt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieormkhd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2elfeiszf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fcrusbek.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2htjfwsvn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psdifdcn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jzrpkwam.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2fssyyyqb.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2cfsrqvhr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rbaxiycm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gtvxbwlj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2avjypash.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2hvbsvppv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ixxjxzzf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2czwpjuwn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2cbsublvm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2cmirygwn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jskglzbe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2hsituzec.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ddthvthr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2gptmmcgx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ygwtodra.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2sdvdxxte.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gwgrdizf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnxwhvhr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2htrziqnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hszyxjyf.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xkkdqsfd.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2zgwdtmbs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2syleplqd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2czgzzaqt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ubjslscf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2spxvdewb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qbudhwxh.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bqdvupsd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cuflotuh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qnclwviv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2grrwhplu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2iuhbgvqm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2tppperic.html

);
来源：http://www.52xcode.cn/Article/details/gt2cvbtkgha.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2iajtvgjo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2sltrshup.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ddeujrcv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zssnereq.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2autwkmlq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ddgtfjoj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jwpedkmc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xkbmcslt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ikvfikis.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2neiprhlv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xpysqsrc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lqugacbs.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2qwtxocmn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lralrubl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2leyinxns.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rnjlwhel.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2uspecrem.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kwmwymql.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2eyesjvjm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2hwdfzarh.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zxnywvho.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2nvixejko.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gfkfnhqm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nuiokbhe.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zszbsstx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2omckmzyb.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ijibznkm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pktnndjh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2vlwndpbk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tgvugnpk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2dirdkivn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2fnogrght.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zhmdxoph.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tpzudyrf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2bvfwqkrh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fjjjgelf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2conqntfp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ismocbld.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2fnpuzdlg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hctvdkin.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vgllyqdq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2mlnjacnl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ldmtizoj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2izryjrgc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zheilpaq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lwfxmnam.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2jidkqnsl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xpexbvfa.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tbxjjyqn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zzzficfh.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2srezovrc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dxraurwy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2vlvsonix.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vjjksctg.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2soelyvpg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pkdvuutj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kwzdmpxy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xufyxaxv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bkfvtuut.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ehftfyfs.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kjzmefbl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ioywbaos.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nphtohwz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2lhhjllus.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2lzujsppc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nrwetlsp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2iznxxtro.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jhfjfcpk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2byjlytru.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2jzmkvcqt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2anvqjwyt.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xlxytqll.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2oqbhkmzi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ksyekxgg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2osowljqt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mklzdatu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xhvfwnuy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2tcntcvwq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2gjlgbzxy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pwscuzgx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mtyfhshs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ssbrzfkn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mmhhftqw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jipjqhbz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2tlgqyggm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2aqieyubv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tvqodjgn.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2swtmmlub.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zevpszaa.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2sthqepxp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2bqccmcda.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nugnfzsd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2huwyuoyp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ksxyvtqa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dtkhaknb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wbutntmy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uhidleiw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2omeichdh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ljhtqhbv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2usylvbxw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2mgxbdjzq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dmbxtejq.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bfpxfqrf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gxuttftj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gsljgtkw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wdpabpqt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2smveaakv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2iwbwseer.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2upzxsrzq.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tnyiosra.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wbligmpn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cwgmbhyt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qzwgvaii.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2drpsevbg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2sebpgnke.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fxgfunow.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cwzymnsl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2izvaihza.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ddogghzs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xuymngan.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fvizhatq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2slozqcog.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ifzhenxy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2flowobzg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2viqnfmqr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2slgvugkh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2shomqxgo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ixlwwqxw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rgykhsds.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2aogutfwv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qadpgmuw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2cpmkqenb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qricromg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2vpmdectx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2iqibyell.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2etnawvxo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2yrfinane.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ggpvczef.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2onppzqin.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lcsgusaj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2itgkzwvr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ojclvizj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wiedpxtn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qmedstmk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2maeimcpe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wfjqegmd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2cverbhyh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xzgjsbjs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2sgibcrsx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2aikjpvmw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gcuffxwg.html


<!-- 参考信息 -->