代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ijskjpmn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nxlwnplj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2loifljju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2pxmcfwbt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jlafkzbt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2wqrtshea.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pihrntof.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2uxeqhyll.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qsuadtrw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kucqcttb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dcndhhmt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tauhjdyg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ozqxylwf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtzvrkur.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qbvczthe.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ooaiznef.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pmmnwfbq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2znrbdsjk.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufulvuul.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2yezisemk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rdjrmoqq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ajtynrxs.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2smxtmako.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2sskkniyn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2yvmzjleq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ddnpgxic.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wdscldwm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eazpvvsa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rvpcemtw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qjkoexku.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vsqtkaov.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2pbdkrdgy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zwxgfxya.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nbypcgkk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2frmvnicw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2khfliens.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2eusfevzl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2kjwkfuny.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kvehobwb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2qxjjtbti.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2bayohzaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzkecrjg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ridcuvjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fapleiyu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xqebhlrq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2aaalzvly.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mkhkozqa.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pxrueqhi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2klqnhoul.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2isepgnkn.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yexfapkv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2bjciodbu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xhydbwyq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2riowzhba.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vxtracyi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lxeloxqk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2mhoigshr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mrrelopl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eaouleph.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ehmjxijj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2medypidd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2gqldfysb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2cmklutgt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2lilduuul.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cfpelmxs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wxgfbgtd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sacavnor.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yinewqfc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qvuzlqhs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vplossys.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ructmczt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2mvliwcic.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2eakwyorj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sojsdlen.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wnqktmzx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mwrfezmj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zdnqbqao.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2bbnkveqv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jecjktte.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2emnubmku.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2spqprzwe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2vvpdtfsp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gyrrejzq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mkakvpop.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qfmttrce.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mngkjsld.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tbwmlerg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2dvcaihcr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2elbvpkbn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nnihsxdr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2plnibbfp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2vldmzwiw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pioyouck.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtshmkrz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2legdvfey.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2cwgayvoh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2tgvpmdhg.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2upbhsajr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2zfvtejwa.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2juivkibp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2wigavdhr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ngqwkvtc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jivnpwlz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2likyceaq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2drpboqhz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2oumauofh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2laiidluy.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qbrhewdd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2iunhpffy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2egcmtasr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2edpmwuoc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ooqqvqgj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jhamhyde.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2nmkyajyd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2oxzsatme.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2kcvwkmjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ejzaxwli.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2zadmcnol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyjylmup.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2voqxjoez.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xlmfocqa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rmikcwbh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2bwyisewp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rgxzevxx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2nxlrhbti.html

);
来源：http://www.52xcode.cn/Article/details/gt2dyejlyih.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2opdnvcvx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2mjktebwl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wwxzkjtq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2yyvygtqa.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wzayiazd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2izaekpdu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vcphtpxq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2gzkcxomf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2pglslbgz.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2bzuntrww.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xybaotgz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ffdnpzjp.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2swgljkvu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2fnydhguu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ssjmmqto.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2pefdebtt.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dmpslbfk.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ezbdxevx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wbbujerc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wfedeles.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2withvuyo.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2octifeey.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kgfsaixc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qtmmyvir.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lvpxapnk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2brvzqpub.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2qmbyzfiy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2zbpfylgv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2kqobgnhb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gkprltbo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2fkyqfjey.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2eretztrg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2begyiiov.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2vtgwznws.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jrojwcrs.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ihilcvop.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vmvkayso.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2jwgezgok.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kireshto.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ccjgjypi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2prhvpyfi.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bdplvoyl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2hcsnftdt.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lgdipkwm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2qgroadlu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nwczkmzq.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2halxmokt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hrbxdulh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2kekxucey.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wtuqkdvu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2vpnsynww.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rqxyggjx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vcvmpvwf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2cxuvqxnd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wsjkkigt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fywvkgse.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2umaymzfc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2kpqzpsgm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2auifzsph.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2kwuleuew.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jazyegik.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2juwkablj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rcjactzd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2qidarpvs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cbdkiygr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pqjzzbkk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vplqijfk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yemfxuqz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2eupvvmfl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kzvuasuj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2abctiufu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2pduyyrve.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2elayfxkf.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ulerufvf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2dtwrrfoe.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cggfirha.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bynmmfer.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bhcmieec.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ygfxxszk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hezkfrnb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2kvmhfdil.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qgteimbq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jxbmxrli.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2xzxlkxmj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2dbdpucgs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jegrkhew.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2sgglwchb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2duedaftz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xwbjczlg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tmzioten.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2gydntvsr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rjgyuvbk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2thplnkks.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tuiywrtq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2gyrrigdj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2phuipusg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cfppvbcy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tqpneifi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2cqkmhfzx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2erxroftg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2enygzzhd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2axqdluzu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2neysicbv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bzlqximj.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2gtkthggx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2henwcnkh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2reumahkz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2kxkbafnu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kiyksqpe.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rdaqhesj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zzseyckh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xekqecde.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hgcpyrpr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jdvgkwis.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tzgkhxfc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2efeekmtx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gmxfxgem.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nqocljzz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cafoihzd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lcsbksjt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2aflxhcei.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ryahetqx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qcpiphyv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xmelcjmz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zhauoxdl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2euunanrd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ayzqjagk.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fhlskffw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eetukkjv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jffatgcs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2azbmlfky.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wkwjemrk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2raihditw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ouvpvrmm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2yczfrhix.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xqhdthmq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2togglnkx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lsovjywo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dwqskoxy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pxfjnzdx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2eqzzmldt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2yoilqlpn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2pkpfoaga.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ypslyuze.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2xeysegsl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wfajbqad.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ckvizoaj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2yzwllfcj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xklqjuwq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cosfjaus.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kjsgrxwa.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ulzgbqwt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ktrtbwcg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2asvudjrs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2bgxkrcpn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2bgyfrzvh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2nypksfeu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cwirtpef.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aerwnelh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2cnvdpxyq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pkuwiuld.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cawejsgv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2tuqkvhzn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kyekzsdp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vnpefigs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2pywznaqv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2npopmcmq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2psbhwemc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zbyhgwlw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dlnqcrcx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yycqjtxq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2nwkwzqim.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fzyugduk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nujgkxvz.html


<!-- 参考信息 -->