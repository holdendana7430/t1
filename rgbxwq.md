代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2jmfuwquy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2punrdwqx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vvliblxi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hovhaehh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mtyqvhmp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2svsjggcn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2erbtzxsl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mulbjgdf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ojdkbyjj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjcoiaq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ilspstmp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2clkaiuar.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2plqycnpv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xyjvtcwc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jhxuaxga.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ueaobgtt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ilhslcfm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zghzzprw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dspmljuk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2unmwcgat.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2upgcmcvz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uokphalw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rdtqbloj.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vzuegzhw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2xhwuymzp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fcouupnx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mvygjqcs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cewrnyej.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2uvgpecrz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2leiuetmw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2lzfcvebx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2yfcqsssg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mrdugeon.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zmrampno.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qngbkqyb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ceshfldj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2jeimatzq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2adkkigcu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2iuerglcy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2fwzgrocn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2hajhwger.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2cazdfjpl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pfkohlmp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bozrvgmo.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rvgblsos.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vnytrwvs.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rboinhlb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ygntecns.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qlhvqkpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqymtkbz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dppfuicc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orvaabrm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wikdxfrq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2zdcrckto.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wcqadnqx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bvtprtej.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2akqdhwqj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ssocfpuc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2blbsokaz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wrjqmgig.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jxksgopw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2rzdaecni.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2sznjaqnh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2okbpfvyi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lwulbzae.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ixmnkoqy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vavadvbt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2jvaycusb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oirdkswu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2tifceoyi.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2wcsjmmko.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2hxjnmmgh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2zecturfs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2xvxxxhul.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2eytcyckf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ouckmlzl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2juzyrxdj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fuguhzec.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fahbjgkv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xajnbxgi.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jddiioan.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2miihicyk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cncyexqs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ccqackbb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ocngcpho.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yzjdjiye.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gkzejnwh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rvylbdbi.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rrcbcxnl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2okufkscj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2gcwiqmjm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mhxzrxah.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pazqdouz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2hkrqbmol.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cyiaekrx.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2paarkvut.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2acdffbmg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2bytwrlbx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jwsgqehh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ilsayzhj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2aypyucpe.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjabhysy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcifffna.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptyuqwfv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ieffmtwe.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kjpuigrg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2sqybmxcd.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rfjkjjuc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lqiyhgtu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pdelcaft.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iwesbibw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrqowmse.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fiaejggw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2eiwkrkls.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2gitufehi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xgfundty.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2oofhftdm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2zslktuqz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2wycyxfhc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qunvpecr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fneaznrw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2frvglbvr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ajtrjora.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2sksavgaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvszbnay.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2bgoqdejw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llqqozct.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2hjhjjssu.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ysohvlbs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rjmhjspm.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ktvuxrgt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2iqcrxuvt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2aftvskch.html

);
来源：http://www.52xcode.cn/Article/details/gt2vxqlzoue.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qzhtuxen.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xijvsqnr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ksqvhlih.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ufjnwzpn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2mrealbjt.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2qzxqhrwd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ilnslymu.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2zsqxfogf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2jawyptyr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2llbolcpp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hygglcxw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2tzempkgv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2jrdwhmdz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2guqkoygf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2pomeyvae.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2pxcgeblo.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jnuywkuo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2grvicbdt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qagahpww.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2grkbswed.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wmeobapa.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2vkgunhjg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2knevghmq.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qzgorqtl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2sownfjur.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2pkublcim.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qrfohqiv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ghefepfr.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2xgwixcta.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2blrhnucw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ihyngavj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2qlrbghkl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2eqblvngh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2pvscrabr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wzjqmvvr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2tfmagxta.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2euancagd.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2grxkmdjf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2epcnlhzb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tebneapm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dloullff.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2rafzdnqz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2hlzvdbqo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2corueofb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hxgfwfaj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hjgxibhf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jtihgdfz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2hvjvgjdm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2qlnyjrvj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bcawuyhg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2jmlfbyfs.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eiswpyua.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzzfejbt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dwwdvhrw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zjslcvwo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jzltylnc.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wztbcsat.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bfmnzozu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2waaxqyax.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2ljknsufu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wlveqaps.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oyhgwroz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvksrpjs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wjqlurvl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cfsvhbws.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2jenxsxzy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2cwdlwcqu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iawjynlj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2byynluob.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vecpsone.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2dkqxzhbe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2hpuzkphp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mtaqzxad.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2iruamoet.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2bagkruqz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zrnibsew.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2nwbcakgv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xpvdynbs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nojqyzji.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2amkjnnbe.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ndetvnzm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mreaphtz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mvehfzbx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nfssnmej.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wwycnejg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2itwarlig.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2uvhthzdb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2eadzbfhz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2wrxveiop.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2pptycjbl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mydnrmyu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2hfnmzigb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ykjbwisa.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qokjmblx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ofrcugrr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mmbmmpjl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2etliekhy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vesabiak.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lfdlydmr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2uivrwsbn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2kynzuqhu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bfmulgjb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2ssnlvjdj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2aqavmgzc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2dxesykvj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ygugqppr.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2shmmrzlh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2pemfjqvu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ehncyvca.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2imagvvub.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2utgwvddp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2eieiawko.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fxwziqid.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2pvhmsrvf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jgmsswfz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2dtlserlp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2iqtxoryp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yecbozky.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gldcwrzv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wjtfuzza.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rqinuavz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2onttvqjp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bpmcyolg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iugdqzxl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hpvwwqmt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kfnbalql.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yrqmkfwg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gtmocawg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mxkolpjc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ybkxcifi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dzkvwbds.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2prwwifux.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qnevhkra.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fahpjiqk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2sbzmasag.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2minplexu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rvicmauj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jxzdgcyt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2uhwmdoop.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qdsbflbg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2epridsqx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ethuxjog.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2lcftedxi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jxchcqfc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tftacbrh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2axsodwwt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2plnfnnut.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lodhlwfg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2hqhlqvyd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wvycxwcl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2swaxmglk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2myvlexxd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mkwrnpmt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ghedprub.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xedxnsyc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bpqykbly.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mtrtahay.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bvqoelgn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ygqmsodx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yulidulz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2khzjpowk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fakucqza.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2oynkktcj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2clrofcok.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yxjcldtd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2pprwqszd.html


<!-- 参考信息 -->