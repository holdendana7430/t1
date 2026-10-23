代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gabwxgms.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fkjzvcia.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3zvrmcdsw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3nhiorsxv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mjadgwhb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fcbscylf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kfifukyd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bdgrhhmc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nknofthd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3swxwkiwe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3eowafctg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3wiranouk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3nsqwgcqg.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cimxprzw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmcdwrs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lxcmcffi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3dedzjsly.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3qorwlift.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3srltfscw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3uaakifbg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3uegxhlrp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3nwftwjas.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tvbqktua.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3smwqbuqb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rurlclgw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zoxamzfu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3otucxucd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kjplgbte.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jfatuhvh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3uwjphspn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fdzmaxlr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rjrqpuxr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xdpcbjls.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mlrbcmlv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3wtwwjron.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3locyzsor.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bnhmeoyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qobjbwdr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3fpmavwso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvqxarxj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3vzndidig.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3uwsiueoy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mmmrotcy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mqzzqqxo.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ojkwbexz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3nxxcigje.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3msiodidz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tuizneny.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3wgxdkgnz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3wvwmulov.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3yqhmrndp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3hxkzduxz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3abmfjjfh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ppuqfuix.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gagjoegq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ptgyrboj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3msdgygrp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3jiwzqmsw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3lfvwoisr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fsfztlia.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3cwaanqzq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tfbbclop.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3juuvihzc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dfgypcxv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3rhgcvpvh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnwerdh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3kmisrtqe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3bzjunkae.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3emiziyma.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fygixbua.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rzxfahwo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pvhnrmnp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ghpdnovq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rtlgckka.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3yrlejsug.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xixkhjeo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3vgfnuelt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3ypsgqrli.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zbhfubfz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3osralfca.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fxbcgdwt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3mkqnutcp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jtvyktiq.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ujnqenxp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3qmlmndng.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wxwsrydn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xcrcrqjg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prxvagsj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ciximgya.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwkvfglc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxeujqtv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3keabvbha.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rhkmycnx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqudmrou.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xsbwspsj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3lslltffz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3yqancmdy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mbzmkioq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3strfqdgs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3tyanlfyu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3uahpxxcr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3uskpbxse.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yzjntsow.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3fgwufoko.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3rsizeiud.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3yhskfjqe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ekmjytgd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bvtjpgcs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ylqsvtpd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3wrqdwkko.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yhsekgvg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3rrirtpth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgczkwxs.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3trycgfqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrxunclr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3tbswsfyj.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3jaggusqe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dqndawvv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3awdjznwf.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3fetgbhag.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3hyiwrkgn.html

);
来源：http://www.52xcode.cn/Article/details/gt3mapkytzn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3gxyqqiqq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3tczblhre.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xaaknnec.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fgfumbue.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hkcqsbuz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hcfaetrr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xmifbpnu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ttiomtbh.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3tixomyyq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3zdkewapc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kvtxakic.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rfeebfed.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ncvjxqch.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lsmjtvtg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fjvdwthh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3urnzqemz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ijrgpnxx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3hcofbeqc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vbqcmloq.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3sscocili.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rwywndij.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3zugovxmn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3oxyqgvzu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3pgruvxoj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3frhxrfuk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wyuyvwis.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wgutfuqb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3cwysmaov.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3jmubffbh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fiiuboum.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vllhrwfp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3kdbugzrt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ofqglopm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3stnkaepm.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tsieprwm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nhptvshw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ewafvhcj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3irxduiwg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hdwwtjpd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3xrwqmbud.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3vkatvolr.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3opylnfgu.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wpiosxhf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3ngahfsnc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3smmjfztq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3calbbswc.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bwdzkxkt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3mqcqditn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3idjygarn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ssjqzxha.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qvpycguo.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vjztmspm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3knctbdwt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3oetokuhn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wjvynnuv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3zymzonrh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wzfwdgcg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3tkbuevrn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvkmjitm.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3panbvofq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vildjrrf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3quglsupt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dqdwviqs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3jzsyhpjv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cjlbvsnw.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wzcggmdr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wsmqiwyu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nafzloia.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3funbfecg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hdyqrykx.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3dfpzwtzs.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3djyynuxo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3wkanpsco.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3sxjkrpoi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3chkaqmtj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3badstaau.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dafxhxuu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zzzhjzlq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3srttxgjt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3prmiryzt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jwzwkspa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3kvizolav.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3dxucfsvn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hkfykavb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3psvonjfz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nequjcqo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3qgvvefmj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3nmlmqecg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3uplecrsw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nldqvkzf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3dqmmevfn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3frodcysg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3uawdoktr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nuesndue.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3fqdcmsyi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3cpsxpnfc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3udxmujgg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mpndqdjd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gqiawjfa.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3dsheazik.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3sngooyle.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mjfntpqp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3tskckvvp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3eigcetqe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3aaibomvc.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3kzbbsgeu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mvomvxkl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3umlwvknk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vqsamejc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hsqchtzv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ovyueyzz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3widqhfwv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3avexywnq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ernxuakl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yqndwiwr.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3pdixeurp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jomvpbwm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3gjomsgfk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yjsmkqie.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3npvgescc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3qprwlvkj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cujzkvzf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lhmtjgue.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3daaediuq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dtwoaiay.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3kpslyznr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hymggiye.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3krodiggd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3brnnihax.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mycbofuo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xuyyelvo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3epikyxoh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xvodovgx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fdkurozl.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3fhewwgfp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pzhgsofr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3kiylztly.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3warheptw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dxkvxpbr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ueitttap.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3noibzpjg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3gegcsexy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3wsrvesjh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3dgrmmvgp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fkbhoual.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ilwwuzca.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qitfniib.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3pknhabwg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3pnmigbsn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hliklqiv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ztpfxanq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nowttmvt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3iujldwar.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3siogxycz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vembzcjl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qiexcwvm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ujbhhajy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3musqdgcb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ivxxcqdk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3fhezrgia.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fsegyhss.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vmkwbqwe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cvmkaxbi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ibwwdahb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hhetihfm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3weespwxb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vqveoxpx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ykvfgklc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3dazunfaa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3inivdzuw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3pvbiiubp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lomqpzpc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pewwpmrl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pfeugype.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3sdsrkyap.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ueibcqsu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xrocwcte.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3goqpjhqe.html


<!-- 参考信息 -->