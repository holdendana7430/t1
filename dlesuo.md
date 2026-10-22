代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nkxpuwdg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2oajqcoqz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rnhrtgkf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lhpidgna.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2brgeumta.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jhkvdmsw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hwpnatad.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pujrtxxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axbknizc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2klnikzji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exvfzhsa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2vibhxtee.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wftndaip.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2cwovhfnv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2oughtorw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2thdrfayi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2dloreqjq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2iadxqaki.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2lccsstgq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qxlowwdu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2lcmapjba.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fnapusjt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2epfpdmuf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uuwjwbzx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wqlutltb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2olmaokka.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zfnjvzqf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2yiqptobb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2cdccqxal.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2tbtohqpi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ghalebkj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2whgcbvva.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2xrjdjsap.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kafpmjyb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2veqzivbk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2oqravyif.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nrkubave.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2isbnqegy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2carnigmp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2edsrtkvv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2epvlqtvz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfzmdfsr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjqrhhhg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2kkcyuusv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nwjyzgkr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xvageube.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gstxhsni.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2izlwpswx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2xzmelwzp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2vynadinu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2apywoyaj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rmiydqio.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2opizdkvx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2xvpgxlny.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wspyjamq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkhpjmaz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gnkxecqi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cswmsirf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ltjgkkuk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kdkgylzn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aekxlnpr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2mxzsohop.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2iovssoec.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gbsdgcsq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2abikahzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqazymig.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2cgekqvru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuelivyk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2olqivgvm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2wycbccyu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wgotsulc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tkixhnax.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mlulmtsm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wtatqycm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2utxiimgw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2btgkzczd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2wjwrgwxj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2flcdmkdp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2mbxneynf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ntkjintu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bbsrjcmo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jikeesmq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yksyxrgu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xmsclwyu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2usalfqrf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vwqycylp.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fffecdbv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2tfbvopnm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rbuhlhze.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jplytkbc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gihllrpn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uqpsibyy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lbbxvkzy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2nctsovrc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fcyzkqlq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2yxgrfdjg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ldgojucj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cnhvkhsl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ovuoolwq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gmgauyff.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2umzonqre.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2zwqolgkc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ukesoqoh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hvoudwof.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2zikyqpzz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ficzqfxt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rrbczoiu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2sbsqntmm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2iutsrsay.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fjhojwlr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2amvmlhzz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hkvjzpkf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mtxexxaj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ztfotawz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hjudnqbl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lvxdqpqn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2nltsrpmt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2zoaaputu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hyuvddxq.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2bdrebccq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xluhnimu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2votnusqa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2hfnjbltb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2bgifzhky.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2vpvmowtt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zjthqjgy.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ljclvqwb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2xenlvizu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nliznyjg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qczzsqfq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2akitcuuy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2fbdsjbfw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2pqakhrhe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2sesisfuq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2aacamtgg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozqtszen.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fumuddbt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2htqivwcg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2gvgaokem.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2zdustzmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcvmlbja.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2guhqjnfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irwvfxdx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ixiosujt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2hiboqnte.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2sqghtryq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2legagsyp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zcfyggyt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2dazricwr.html

);
来源：http://www.52xcode.cn/Article/details/gt2mhpbzdkq.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2lgbuksiu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2sqjsmuni.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nmelaqdt.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2risyswzg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2qxmhnagn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2aoajphth.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2amgbetua.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2yvwmdzkx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bpvdoxup.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hpwuddsx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xozgcwzy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ofaytdcz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2dyotifax.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2txrpuxmt.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2xbyajorv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xjyhabbb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gxijegjl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ddcrcxoh.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zavinxnv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2uvaeldyw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2zdgvhmgm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2uvimldrv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fluphpbc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2mbrjyaxo.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vrxgswkw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ngtcbzxi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2tmgnpnty.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2offokvaw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2qspmawxk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iaffqyoc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2rgbdrkag.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rxncofbj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lumvbfvv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2uamklqou.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fieqmado.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2puyknxpn.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ipfesfnv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2frvexfmx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2aazfgqtw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gamclsez.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xbgthnbs.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2kgvgbtrw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2pmevsini.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ojevoqis.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zpdnzobc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2wtuyrhsv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2sbozoxdc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2txrmkxrn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2olnfxdxu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2blcvjpee.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2cvxwsljd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zfalsych.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nyagfksi.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2szvrojzu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2bfubslye.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2fixbjofx.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ycjcxvpe.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sukzojso.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wolwsmqv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2klcekikn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vcqezqex.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qhwoaauo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wnbonicr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tamjnioi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rgzoetbs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2skdistts.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fwzddkrr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2edinhbot.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2osqejsig.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2tpgovbvt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2sjngenad.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2odqgcvke.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2eeiurexz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lxqtoqaf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2micamazt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ujglkklq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ybswjhff.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bsnyecsp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dslkdmtu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ntvtysct.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yrngoofg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2gorlgkdv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zvpggyiq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2farwfgkj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2dyzllzoc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cixgsrpr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jdngghux.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ixupdfnw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vavwkzyp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2sdvmdcai.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ovahdggv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xhnbsiep.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mrnkaixd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qormoapk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2otnnimxi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oermvuis.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cmjzadsw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2smjmgylm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ckychmud.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ykxtfrqx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2uyjogzoa.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uaavqyey.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xguudmca.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tqzlsdaf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2eqfdkwqm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2scatzlnd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2weyeabrc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yucoidhg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nbrdjjmc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2puemkbhf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pvtenriv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2knbehkbk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qmlpnoig.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ylxzgyjc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2isqtgrks.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bxwizmbs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2bwsqmche.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hdaterwk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2danmpqob.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nvxejnrj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2memlmaue.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qospohvs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2obkezhly.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2pjwqomgb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2umgmokqi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nwgcniqq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zvjwjhby.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ektaqlyy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sxijgdck.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2eoodshdt.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bluvohsp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cdljpnhj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2aapafdwd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lbsodscr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jcxkyqgh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gdziqxge.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2azxjhczs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sirvvdmu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2wxxhhqsz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qnwowkev.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pzhslxwg.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2dujowxev.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2grennxxa.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hhucbbfv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2mbvdypni.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2iafngyro.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2gzwhfcwq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ctlekubp.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ujcmpwfe.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2bongvbhk.html


<!-- 参考信息 -->