代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fckfvmej.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ljvvsyez.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3jvotpnrq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3grukxkrd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dqdcjgsc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3giycvkxh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jjlugped.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3dfflctan.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yieneahs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ryaeursy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3memjzgdt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gcaaerrr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lhyplzty.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nrfptooy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3txbrmman.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bcsmaafd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3gqfbduug.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kihdxkvo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bynsstbn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3zaazhxmi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3trlhxmks.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dfdfycku.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwxhjrvq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nkhvsoop.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3isyugrge.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzvywsur.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3muzomdty.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vvrdiiwl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3abflrpxf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zivqgslr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3irxadama.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rjdemcuv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3pskumymk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3wdskqasl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3seiprehb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qmvnjhps.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qmcebkzu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uhlhhnri.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rlfagepn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hvxmvkrf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3uysbdtcy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ecmruhyf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nlvcvhvd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3pbwpqhcg.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qmqfkvym.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3phvvvhih.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3krnpgely.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lvwyucvo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kdodafnf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3txjcamvc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kvdxjatt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hkvzicsn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cjnejfjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqzjomvd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dyikhkjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zacnstab.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dorsmnuh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3znvnbbhy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3znlghwec.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dpetgiqv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lsrxdera.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cslritwu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3nhvjgtol.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jzgpetfc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3peqznvcl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vcpvqawy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mzxolwoc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vsanaeww.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jjbqxsuc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wnmhkytj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wcttipkm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3tgvidqlh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3pupcbsiw.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tpyalzxi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3csnvtbuz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3guhjscus.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yirhnjww.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xifzetni.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jmnlfmca.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mndykqnt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3hmssdufr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3psbpntqu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3resmlwii.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3uqorxfdy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pfawayrz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wlgdnoip.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zfiiragk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uklbnxmx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ktxazpom.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3tfimhiub.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gxlkshjf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3blwfcpjw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3petrohsv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3oqwoqizm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3xdytjfze.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3nvicunvo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3aomyoaio.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3xmhslass.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qcjzlmro.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xmlvtsin.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gpdrgvzq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3mjxqxfjf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gajfovyq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgdrawrr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3mjzesmtl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbvwyhnj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swzjgnsn.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3mbcacylz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3sygxvcya.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3vzedzdst.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3iyublixs.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zlwzqwdr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3faxnzjqb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cnkehvld.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pabxpaen.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpyjszyv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3wyzohnbq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rqfmktjy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3seppsiqv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3dtohnmsl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ascptwoe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3orocaeji.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3fgouujid.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3shaumbsm.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wiuqdncf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3icqcgsjf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3awazqfiv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3xnjyjmjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkhklgcx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3odukvyey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evlbbjkt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mqkjyuqf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jdcbmqaz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uxpgsbrl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3zhhknzbm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3jkgimdou.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3dycnqjrz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3obidwhdz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3oqevjlcr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3erlpolwj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ksvojadd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3uqbfidaa.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3uodaenja.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pyjeblub.html

);
来源：http://www.52xcode.cn/Article/details/gt3smvqcclh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3lfprzmhu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cxzlbgiw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3wwdctyxr.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hmpuavbl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3thnoosxl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3rgcztzix.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xpxdsied.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fucgybyy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xerbokra.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kmiqimih.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3podigutc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fbfeftux.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3jybimfrm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3mdpmngkz.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3zuaqnloa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yldshaoo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3flnjpqew.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sozhzifg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3nbxojgns.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yptkdckc.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qibmjzdv.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3oompojnb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nmackjud.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3omdlgnjg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ohjqcszu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ixmllljk.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dflrflxs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3goaqgvac.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3tvmsdbsv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldvmavaw.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zlevdsdn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mqbajvjj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3vehvizzw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3eukalbaz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3kxlzbaee.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zhtleykf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zkmkwpiw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3enxurnfp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zcytjqvh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yqufoezs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3urucjiqz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xycjlgdk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cmefngxq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3uziicxyf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zelsgely.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pucxbrmh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3wxpqriyo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qdfhpndo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3fkxjwbuq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ppjpmpoc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kohdwgvx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbpvdcpl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3icptalqi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cgpmcnir.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cwlplxne.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rydcxwia.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fbkhvgcp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ydhqdncq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gpvwcjze.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3hrhuxmwa.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hakgvgat.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pxdccpkp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3laaxicwk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3aavzozqk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3zubvqphj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kjycllai.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3jqieptgg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3calsqdug.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3otfkkbgs.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3aunxypnf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3txczmeev.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3omkfhlwz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3eywtoiwz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3dtsdjgwn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ldyyguwy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3pnoyiadf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3yvzmvkbe.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3sabulqhl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3clkmpdll.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3opcvvuqe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ufvnsakz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3zlxvufbd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xrczfbcv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3asyfjhgp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3omflhaqb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zienmict.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3hltiipfs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3sgjxkhww.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zepwlnlz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ddtpbteq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3uzcjuirr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3wwbhhuvh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3bftuvfxz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ymnurfed.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rqefgnqp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3vfveridw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ujuxicdt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rbwqkdwm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3pfvhxptn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3scmmgdih.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3asuiarov.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bcoovvsv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nkppijvd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3crdzhcen.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cdskxbhg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tpovjomz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3uvyuwklx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3xzpwqpzv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3yolrodhb.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3njnbtcuh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3kpsinuaa.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3etsjcjsa.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nhgwired.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3yvbbyjli.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rlwahoqx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wjoakcsl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3qzxbeesk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3inzopkum.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3dtvfgxkc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3liuesghl.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zqmfkxpg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ybkpfjjr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3eqrslqrv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qlqdjyoq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dgrjetat.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3tystvtab.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lsjljvfh.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3kdomafae.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eanuyjwl.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3iqkpdfcq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bjxyqpyd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xfmfftoo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3pgulosjg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3atahopvu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vfwdmcqc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hecrilsa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3xksjyopy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dtkwxcfr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hyeqcftd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3sfsjrhkn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gnunpgqs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xgobyzch.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3oxfrtxss.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tcttpagt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3hfabyyro.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wuuupjpq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3fqbfauwm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ypglbrti.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3yejzwxqx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3iwicpujq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3fnfbudiz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jsdscyer.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3syydmnsh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3lwlynfgg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3lnyshrse.html


<!-- 参考信息 -->