代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jojjhrfx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ihiycuvs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qzyqfhfj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jipmxcxd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gbngxokl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2fqtunmaf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2elamufnw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2nqabexvw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2omsivhsv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rhyzdihe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdfjuckv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gdcoxzyc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nllcmsmt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vqhzmnls.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2wncuqonm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2dxjwxhlz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vlnulkue.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdqhckqa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcozxed.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jxhczbyu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2iyclaoum.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2gtrpineo.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2mmqvdaya.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2trjiclmm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vpgjwsdf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ombhpuzf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nrrmosaw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2uuzpebhn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2forhlwmi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2afhpalyk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrhfggg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2npuaxkco.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rkbjsyhp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2yjnwuabo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qbwcymae.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dqgmszgt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wkflcqka.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2jnfyutic.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2oywacjxb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2nhnfwpqa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2mygxeuif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daoqvrvr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kyjlactf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqixqbyl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pbitksfn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gjbbazsp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rolptcyp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ebmuvqch.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2dqbwjnde.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2uzrwmtph.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nbuujxiq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2yfwzyuzo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gcxldnaz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qeufkgfc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pxmkodsw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmarukrd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2yqxuehqw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2klosevis.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zxfyinuy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2sqyotuhp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfgalzbi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2oosetmcr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2rcvumdyx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2brdbpvqa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2geavtopf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iqpcvhwe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2iptrmgbd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vatmwhpc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2arpmjoin.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2wdutykbz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ewxyvjop.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2zimnqhrj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tavpoiox.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2smjwrqqi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nkfiebif.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dzflpxea.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bsyzwlqm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qavrtnqb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lrizcijt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2thlengfk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2dkczozsm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vaolsoib.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2xsipvqyq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2bgnawjsv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2sqazhajy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2tzazqcdo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kehutdqv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ituloowh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xexonqqg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2chsszakv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zdbuxafh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2gaglthti.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2gfnlcleg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crnnaifa.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbdbsyoq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2hcnvccpi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2fghpvfsz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2udvsxzke.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ucreqaon.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2vhgxrbav.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ydgvozas.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2squlzzdq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yzelzzzr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqfquwxs.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nllikdlk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2jqpydytg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mopdtkif.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2bvqsjphr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2gkhjoiqt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2gwtpnvtq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2takaupkj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jyqqdgmb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2jbukdjto.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2mzosfbnq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rbnodzoz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2eadptmun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjhlwlce.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tprdbdge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtnndwkw.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2avbjloag.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2cuwzskog.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2pykowtmd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dfgmdglt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zfvxenip.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xqqfhuto.html

);
来源：http://www.52xcode.cn/Article/details/gt2oxaqeslo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hmftqakr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2olgghfla.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xbxziouy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wutezaxi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2lojothje.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fvrczqiv.html

);
来源：http://www.52xcode.cn/Article/details/gt2vfeyfnnk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vwylacxt.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rdxfmgcc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kzktpogh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zdndlzxp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2eljvqjdf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2pzuolvrm.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2tkjfyekb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2armasyox.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2agtiktrk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nezamogb.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2eogpcgir.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2drqjimdl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gjazrmml.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2neoliwwf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2bpxvqwhg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mimdznfv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nthwcevl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2yhbsgmvu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2crzlvnic.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2olcdrzas.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rcxkqteu.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jbsgkskl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2riiesitu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2absqlgxx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2gcqrrwip.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2tiyasgbk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2qyakxqmr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kvamdodw.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fzsauerb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bxrznfux.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2jjqkcpbk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cjxjgkya.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dehvtcez.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hkimmgnm.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ldwpkfae.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2nrtjdrca.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2rptcrqfh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mvqmxnxa.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2manjkbtp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vvprcjux.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2nmrrjjpu.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2tefvijzq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2riewniqq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fttmnaqx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2euzbttwm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2airzrdwz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fkelmfmg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qqlyyyry.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vnglxauw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sfvhugxa.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mipwttkb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2futzjfwe.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2umauyjqg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mvirmars.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rrjlqlll.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2owgzdecl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bbinquwd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vjahremd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tbogqtrl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mujpyfqr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dwjwhddh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aivoozzh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2weqtzhot.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2xwtfcjeq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2msjfgghz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2oibegzqm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2evamrzqx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dnkandnh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hsgfusxy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xsctabip.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2joaayhmf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ilxvcqcp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gdsudfai.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zonxesnt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bfjmubev.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pzdgmbsc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oshpvzam.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2yudzrhit.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2uebclxaa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bpkwojaw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gohftqlj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vtjnerzm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xpmqwbji.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ztsqbkwy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xgzsfyav.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zxmcebam.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ulvcrjzu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ksssnbkt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xzodegjf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2pklcnrvb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mnsxhhfi.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dqxnduyv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2cdwyksuq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2tiqezxuj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lvwxycfv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ttlhyykt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dlhoceua.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xbxdusvz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2spfjkmwv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zlgcbdqs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ofzjtlzk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hduectmn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ytojbgkf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sakhcqgn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ewrlgecy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jwdsfdcr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2rynaukhk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qtfyijbs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xpjgkutl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rbbnvyqp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2oenzebkc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fpfqbfnj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ipcirfup.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qfeaprzz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vnkcgbyz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mtaunony.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2haksztbj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2jcuwhgqj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wegytmkj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hejzrykf.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zuvzslgu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2julqprhu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wphdxllp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2adrqghdb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2aakrarjl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2jbcnbloh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hcnvztnq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xesjpcoo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nfhmgorm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2iqfythzs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bolnmwsv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2fatfxymj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ywdgflpf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2sclhpwqr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2zlokeekr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2zcrvlulp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zymnlisq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lewqqwmn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qnxvtejz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2nisbvqae.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2xkztiwbr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2tqugybpe.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2isxldtqs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yfocaqlv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lmuiefpj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2cfbpjrqb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2uxbkjvip.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mnrohjwz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ntprpaaj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pzzqqzat.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jpbdwcbh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlpyizga.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zuibczop.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2voxpzsov.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mradzygn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2rbxrjdjf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fgcsccum.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ftlonawu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zllituoz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mccyjbhu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vcnxldum.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2trpzuetr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kfkbduwg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pmzddjxw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2muvjkxot.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2klrcgtjd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2nduufqhh.html


<!-- 参考信息 -->