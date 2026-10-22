代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2nhmlwdnj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ntalsuyc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hxltpbhk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2gndgtppx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fhbbuoao.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jlmecdtf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2stghofee.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2esycrphq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xguxuest.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gjwfwfsi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdedbevz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2azpljqna.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2txpnqqfo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vihisckb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2stmkwnes.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ppojnmrx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2qkhsioes.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dqhncowe.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zotbkpht.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ruqvupgy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qntarjhu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2svyeomoz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ekkmvcch.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2glspazyx.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hqaazjbg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xfmjxzkz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2bnidsxaw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ntnmzsjs.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2wadavcyy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2odefjhpy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qckdncqy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rkfpwaiw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uogbsuwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onfaeymv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kampecuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgvqhhwz.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hcvrkves.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jtgbswgj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2frcsfgmj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cueeytnt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sdgefdst.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rnhcwotz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mongtsos.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tgrukhxw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2iednqihw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2fncpxvop.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mbcwdofu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tnlagqdv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lnyxzmib.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mulchxlf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nxasonjj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2uwwtseiv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldcunxxu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rrjtjqdr.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dtcwozfv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ehewpggl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2mrkwmeec.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hkxnvxzk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lldeitpm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rjtvedbv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2uxvlztis.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uytwduai.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2pjxmjzzv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vcpepxrt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2sonvgdmj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jyultgvk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fuedguzv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2eczbkzvn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2etgzqmqi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2vfmcwstm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2znkfwqyl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sxgjzwdn.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wdjgosvp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2uunytmxl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2fsuyrvhx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2lvihkkus.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qsdwlmqs.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2aqdjptqi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wlnehtvx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dhhkzatu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qznlqtgp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2kgueyqax.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pkuuosjk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vqrfubsz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2qkxclfwr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrdseoxd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qaeylvns.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2fcxlmhvp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pxtchymv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zawasoak.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2bmxmfeke.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2utdpxuof.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2jtqzgkex.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vgtmclak.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hsolmteh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2vsxaqmnj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2yncikwoo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2bqfregcj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2ettcnthp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jxcuvrpv.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kysrtiqz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2pdwgrjdk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wagvwafb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jziybgyr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ekffoncb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2gdbuxkth.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2egwgsjda.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2siunznwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkrqqlpy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kcxrejkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwpbpmto.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2vxsbfwhw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wwknctgw.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kiuhurxk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2iiojkpdh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2avziypqh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2dnmvacll.html

);
来源：http://www.52xcode.cn/Article/details/gt2xwfjvbrn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2wrtlciod.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2itohxkzg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lfpdrrte.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nrckjeoj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ghbscvrb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2xziodtei.html

);
来源：http://www.52xcode.cn/Article/details/gt2lfnuwtmx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vlrnvjms.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gdjyssxd.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2zchqhkku.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qidcmqpj.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kgzkttin.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2opsqljzz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gliviiez.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qiqqsukh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2facpopri.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tpcdstvt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yzphptxk.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lzdazhgn.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xhrvuxoc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wmrrlhln.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2zxixlabl.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2guqwnpps.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wbgybdir.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2genvbtth.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ljmcyjhv.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ortvkfeq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2aoctskes.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xppyuris.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2huqycpuz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2gsaanfne.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2qykljozm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2iccbxhjb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dvrpwjip.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rixweyhu.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2khlpvcmf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gmgiyikr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2duehuyzk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ieddaptz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dypsbdbj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2npujipsb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2pqykyftg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2iirdfiou.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rwkcdtiq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2wpvyvtnp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ggluheln.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bijofwqt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2mggmcvjw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2owtoohmz.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wqjbqacn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2nrjlsiqv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xetivmjo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sfihibqp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2rzfihzim.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vswsebrf.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2gtvhswpl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2olyzbdhp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2aqjkgexw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vbnjwacg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gceqgwet.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lfxdjjpo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bjzucxpl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cxsfnxgb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2wvnlrszi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2swpjcode.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qsvgvlay.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mkydhahe.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nhdlgcuh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mvzafwoi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hftyzyjz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2cvbwsslv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2tkbhmrtm.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ncpsddzw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2vfygoqsj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wmxpslli.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qeskiiir.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2subqqnik.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jcfrqapd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zbqowmnd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kwassnfl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2tnhdwplh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hlpyvadm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jmifqpfb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xxwzuifb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pigmxzlt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ipbigzuo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nqvkcbff.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2fgwppfvd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2aihogxii.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zgtykoeg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2juhckbhz.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2igjojaij.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vawgbirr.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nhqpkxnt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2hshntokd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2ndvfobdn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xdvuqjub.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2nsfhjzoy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2tuiinvll.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jvfojiko.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2bwlnnmxz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2akdemhpb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jfajunjh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2idmxpeak.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xqwjzqmo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2euvsqvxy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mbnjkdkv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ajntssls.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2aagnpktc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2tumviqcu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2knjeekps.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fvhrflhn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2svrzpddo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2mwourobv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vlmtlrnt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rkudokqq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2scvtoosg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2osvqvqts.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qokbvbko.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2iqomgdfh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cdhruaqw.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hkujtbbs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2imwfijqo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cgfsvkfw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vlubaoro.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2poimofar.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lravnmaz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2nmehtmcu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ifhwcbju.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hpcfngmc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sigkfatz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2isjujyns.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2zrudddax.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ksooagpf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vjqcmbsa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hernkwoc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ecvnvqhg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ehvhnnwp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2mdplkmyx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dqvztyxo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vdlodyde.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bgnzcsox.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2qymzdxjl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lqoclxxf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2opjesfzt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2umtvnhli.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2wnuycofn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vjcenczf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2fsvnkdxh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aurgdeki.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2htjgcimz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nfbvhtms.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jegbhrmk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dpbvplhc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2huxddqkv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2idopujvg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jbytnfnm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ngsgzjwy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vqawczdj.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wpvdfehd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2klkwfvum.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2bqwmkuld.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yfxoaemj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nbirdexy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2duflphfr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2objngylk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2gpaktszl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2acggtghp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wxcrrvah.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2wjrpjlxo.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2udzkbucu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2zgiupjzl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tuhmqifz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2epswsjgb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2lzimueqs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rvagyouy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2bltphjxm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kddnwggu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2irockkvg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uefxopjg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xymygibe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2axvgzkln.html


<!-- 参考信息 -->