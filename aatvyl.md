代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2nulptweb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wiuhshue.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqtihukv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2wlyuhbpu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dnrojydl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioujctmt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gpydmotn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2lwwnrwwc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2etunrcfn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbknmnvg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2agfbtdqr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2tvobfjkh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2hdtjhobz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2voxybtdw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2bmhakady.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2usxxdius.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jzudaogt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2oxmmytmc.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lqzgvttz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqshsvy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2sviiyuyn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2isxtshpm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2daszpacb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2svnaxiuo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2vtganfak.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lziptgrd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ygbufryc.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zbdiehge.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2coixvidm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2wjsxnnzu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tlzukdgj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xoaqmdpi.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2uboqwbbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyvparcl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2cqnfeoog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pouyrcai.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ldvyqecr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zibxtlyk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2cyznwsss.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lfhgtpyf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oezxkwnd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2putmmdgx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ogfkgqkh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2woyjytsm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2cofwsfwx.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2typxpgbo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mbodfjjj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ycojjkww.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2xqajwlpd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2neycktcm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jrzhojfw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2gabcvnss.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmimjpxh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2nnybaujr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2crlfxqtv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zqpwxept.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2dcdepcai.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xlblhdmk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zduolnab.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vahltolg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ivschmnc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tsufrnbj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ckeuydjn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zxzqamgw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2xobppqcc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kuqmrkik.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qflyjbcb.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vrlpixih.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2acvzwklo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fjlrhhhb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2laetpttf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2scpyskii.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ocbtiter.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2sfsdijwf.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2dihuevti.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ylqjeocu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2icxhmhkd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ckhahsgk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oyavwywo.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nkdabari.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2fmxanoaw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jqcqtpyg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2sgnojhnq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tqfbkddb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jtekwtpc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2wadeurbt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbwgtvlj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2llcxddqn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jebnkphd.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ddtxzfuu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tbewbjvv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2dwsulcks.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vdazvukb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xbvzdixd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ealcnqvn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2fkmyfakj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2eekbczzc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2guezeqfj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vpckojpo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2kqhlzvfs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zbfourcb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2amxlatjn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2rlppjkgb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvfgpyqa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2henmtnnl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2pfgmfptw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2sdxweehi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2oraiuguz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luceemvk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qekkjdpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewzyegcl.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dzbksqyh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tvydgpoa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hfcffgaj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ydlcetki.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bhcvcozk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2sitcrrvr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2yotieegp.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bucexcox.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2zsgxwqvg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ksveqesr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2seuhoyez.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2yxwmhkie.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ipphselj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zioebibz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vjsrkefp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wbjumamv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxcwpxwy.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qtypvcdd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2mfqivzrz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vrbdjass.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ndrpugik.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wbmwlxxz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2lwroazaw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2suxvppyn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2wvpyarup.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nmxebzun.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2glyvmhia.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pmendqkt.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vzfrvzxm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ygbyjtiq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wjihvxnb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cxdpcvok.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rkzzizld.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2gfyvutce.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ycssngev.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xbmwzuop.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wsbjepww.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2wwxcapns.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lbmfmbcq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2cgordupr.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ygzksrkb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hoowlhle.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2jezqrldl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cittftry.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2hxchpgcl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2drklkjcw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gkqxbgbo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2mpcuzpad.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qwdgqnyt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qhxdsyxh.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ecydewlk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2msjqllue.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bwojiibb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kappzesk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ovspsxmi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2zearmujr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2muyqrkbv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2crebizqx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2uyabcxbq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uifnqbjk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2tgqiutbl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2budvzbxe.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ukwflrab.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rhdfuqzh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2axnyaueq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fqwszksb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nvxrmgfz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2akprnlbt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2nmujetqc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nbuqypyb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vpyapnzm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qboassax.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dzabskdp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yevfpwzp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kwfrkeqw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zeoiyoum.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2clkzzkoq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2uyrfvugm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2iaaxjsdh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qvzdzhrl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fpyuuxkt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2erkqpdts.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2iuquzcep.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2pbjoxqbi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lfunfpby.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2msoqfhpk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ieemajub.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2arufqisv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2imcsizvy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jyptzewt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2axbkrxdp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qbdrawdn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eghwdngf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2srqxrspv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jgaanmla.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2oqyqfcej.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hcrulwju.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mnaszoca.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hxulcrdk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tvbbhwyh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vixbtfje.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2sntjhrrb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fymqpeag.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2senydxrm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2txkhyspl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qbsavajd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2yjzeepcm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vcirwykw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2mrjnqumu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2oxrfzcuc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2yuhrlqpe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2yrjaezel.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zujhyrkr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zdiedfgh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pfnfrris.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2etjutddk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2dywarigr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2whmugsap.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rpwvxljb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rsumlygb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2bwlqwhck.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ujdfkkuj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2pexntsxj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rnzrnmnn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2knrudagt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hkawpfob.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2motorxqg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qawhnmdl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2rbfonpya.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xpxijfhb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2grzlreme.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nywqkbda.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2yfeiuarm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qmqxkgma.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qctmyjgk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fqqwjtpf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ghdhezvh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pufhexam.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2iitfqhyl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2yrjtbfvi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vsnqbwhu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2cniblrvb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2escvaczl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hepjseuw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ejggpaye.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2sftuwknv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wurtutjf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lgjuokiv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2noxgfngs.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2bemcazam.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2pthxaznz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qmcdgnfg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2thbcbzcg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qayagyga.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rkeukfwm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2riecpvzl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ljathbyz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dvngueiq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ruizwzuo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2edthnfcm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ksemdscw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdthjuvf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cnsinplh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2wtsddfoa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2berdoidq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zdqrlypi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xpygkxpi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2opqlulcg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gryzdazi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2icgbwzno.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tsaflkrh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vcocifhp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ebrxkugq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2enmpvznk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nhwskijo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2paewvjaq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2uosclunh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nzlvcfju.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jncmgosa.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ibrjrmgo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kknveexq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dbxtvmnw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hfzhmeyj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2eookaiiu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aczaaouj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dxmapwtm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nkvtyzpq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bwymdfug.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wybowkow.html


<!-- 参考信息 -->