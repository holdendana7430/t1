代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2rbrsolmg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2takmvdji.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xdmojthv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jjneymer.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2eklbymxe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wwmtsrtf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hivztgjx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qgmylffc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zowpxygh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybxrniwt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xwfkxddr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2trojgkcs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2oxhqmhst.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2arkaintw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2beiysixc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2prvkgojg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fapcuhjy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2zfmeihhc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqcxnuum.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lcbabtlg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nijzktoy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ydwwshlz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bjhqeybj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2djzxkoqf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mwvypctr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qcxypidt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fbedwuas.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ytldfcmu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dmsawmwy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2rhgjshxu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vpmeizrr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2janqtext.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2uvyhpmsh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ctbqrlgs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2afdnston.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2cknxiarv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2lssmfwsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjxhnabq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2psjkjxkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgakopeu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vjacyytr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2kemjwggq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2kefmhmkg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2icxmcthj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rdpociri.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2jcslhwsw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hgzjmsqe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2usyugqkf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2iarndkzh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xznabnqz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2yjkrqagi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2gorjtvhv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2sjvjwoma.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qekmjydn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2aikueceg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gmuobatq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2uexjtvhe.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2dusojvwa.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yvvzgrqk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2qdpnaend.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2crktnwiq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ozdaptkt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yrwztala.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ffutmqya.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ybprenii.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sdpchptf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2pzbssibe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vxrjfevk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2pnggzrsv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fuzlmidr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2niskuhcb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nwatlqns.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tjhohquq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2veoyvrpg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hbpzzpnq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zhfuhxlh.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qvzasshh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rhsvupov.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rhdwxkcp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2eszuuojg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ebgrevdl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2grijevnf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uirhtgdy.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2duhtkbbz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2blreivwf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2tfxdfpej.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rbdztxst.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hbjpzmol.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dwgmvexp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2wpqysfib.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xcackikh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2iycjrzwo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rrtamssy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ybhnhwbp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rvacgqyt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zyoypgou.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wylqjcmf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kwgsaryp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dbzltpqg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rsjnvcfx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2eaypnjat.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2shpohefk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2nrhbzucn.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xlvvnvxn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ebzkvrwv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zqzapsfn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2digtdnqz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kpjxxsnj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qxexxmhf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2greyavpm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ynuizqli.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2onflkrob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvbfdhgd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kjlvvfil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvrrpqtp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2sedcdntf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2txixczek.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2amqqsitg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bkfeknhl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2mstqxsoq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2rrjuklwu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ilzbclqh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ishcnnaa.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2lybsygxx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2euepbnla.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pqwxzrvp.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2fzkoyufp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mnyrohcc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wudnrlmc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2qrbfltxu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nihlbpbp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2hniwfhfj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gywpjpht.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zniumnfu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ejslxfci.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2qinjqlke.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2avhkjluc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2witwpirm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2mudekqxy.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2kdoufmff.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qoaahjyw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2quvqthxd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2daabbkwr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2zojtnvyx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2izvgrfwy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2wrahyswq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tttoltsv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ddwlfnxq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wjemqdsq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2fbyqqvaz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2asheridj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2upzpuuzo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2rnmvapuw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2yakbdfma.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2sttxdkkt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2uzhyddst.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ypdpvupg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dgubvpom.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mgbzhjyh.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2sywoqjoj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2daqdsztu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2glktrruv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rolzlhjh.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tgdseghz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2uzzvfcep.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xlirwmhr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ojzeovcu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2jzhasxgk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fcyfgbwk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2vfifevye.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2hrhhgocb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gbhcntvx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2gekfsqgt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2phdknpyr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjlnyden.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xufsoeuc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nowgvips.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2yhdjjots.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oliacpfk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2pdokqtsc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktjytcsp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hmxrqsqe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nupjekwd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2foyakvha.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hnvqcmph.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wttkukli.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bnurolgm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qtluwdof.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gdpmijvn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2otpadxho.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lsfpzefd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2xxpfkjmi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qdbdqzzd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gukrsvko.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2dytthelv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2xzrhulzk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2uliiacgx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ltcfvjhm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2leqypjox.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zlbfifrz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ybqqvvgs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ktnozeff.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2gicatfla.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2pixcclco.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2uprymqtz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wvswlswz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2mftfspyp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eaajawwv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dfgplhhd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2qpfaxyez.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vjtcfkye.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2admomjhm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2yroxywkk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2bxwrsyhm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mxzpuans.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ohohmuoh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dexmqojb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yvmxhohv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kvrhxcnb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2khkiwdqf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pgclchvv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2sraokxxa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2hnkxhbkp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mjghayez.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gimkwoiu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2efqztvjn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2iocbvzbs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2wpyjucmh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lsaxvhjp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2nrkwqopr.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ccovxrjs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2oipcujgg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2avdbfrdg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2tbvblheo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bhtkmxlu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mbembfmn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tguwzlni.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2lpjpufwv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xupdqovn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wpfsivnv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mvbqminy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fuuejyqe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wycqnmhy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ukrnhguu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2horkwnuo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2exkfrrkl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ywcirigq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mxjslslw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsinsvzu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zhehnewq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2efgjettj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ykvbxsny.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2klashien.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nvubzuaj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2orjodpse.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2umuljdbs.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zmmhjfdw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gtsmgubx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2yjdthgdn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lndqesfz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lrrgnxij.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ehpxclwk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2cghmjmyl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2iusevmme.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2bichmdlo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vobfuzye.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tcmdrfsz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bbsjxmpf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2sqnsgxfr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gdebasgz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qrngpbff.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2aifympvw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2uzphawvg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2sjuuxppl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jpxfalgk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2trujkyzd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xpobeqxh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2twbdjqvy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mxyemymf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2trchtnju.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dghbosod.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2buauquxw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2snvyjurg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2yzmynbdd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wbcgjnwz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yxtcjziv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jatgclxp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nybwhrjx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lawrcobi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rveyhotz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zpmpcopi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dkxlugbu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2arehotjb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ktdtviwq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xfkiucca.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ettqsapo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qdjmopzz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xslwtslp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2yzizjbvn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ixumaipw.html


<!-- 参考信息 -->