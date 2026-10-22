代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rckxvygt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2prgqxtqr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2chwzkvar.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fernrjod.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ffmxqibx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wnubehzg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fofpsxjp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2oquplssb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffknwdwi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2nsbcbgxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2damovfjk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dvaaekav.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2hqszamoo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wgjoeexq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2jdqiypkm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jmphmrja.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cerislwd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yfciniel.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2flblmolk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bwukdpyw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2efvgsagr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ipwpofle.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rkuujtfz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xbdebxid.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xfllljrs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rqdiixwr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2kaqdbgfk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2xobrgeyp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2mjfgknir.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2akzsxghz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tdjrsxgu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2frktymac.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2chnykmwg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ihooyyhl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvehpis.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2yvondrrk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2uescjkrw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2psdbtpqf.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pnzvbhvy.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lgyxmuhh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tjqybwos.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mxhcefya.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckcpwecz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2krucwicx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2dczdysna.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2sksritye.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2wsfwszsi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wfmlfhao.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cejzfptm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2muvzanzt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2axldlfor.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zobqiijr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2yblzigie.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2grkmxjqr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dpudtyiq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzvyutuw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ufwyfqgb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2sevynrtx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ovtoqchu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ukyxothv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kaftxadr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dlwykvmi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gcpgdzkl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jqcucokv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2cepdnjoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bskiotsq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2kkixsycl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbrvyotk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2djntelga.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2cixcaraz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2sqaxuakw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rhtobfar.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mhbwrxex.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ndlzqtvm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xlghkyby.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fhvhguxn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hczsytxg.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2sruqpbtq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2dymkrchu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ckkbacgc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2rybwgchi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2sjjczmie.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2byrklkzk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2txctqmoc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2nutsuqvh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2nokggmkf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ctyhnsql.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2dxfgqpga.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2gkynspss.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2glwckept.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hakdyezp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xdgwhlwj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nykjgjuq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ccxpufjg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pkevgrzl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2epwwmnzq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wiaypiym.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fugrvsnq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cjdwpcef.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xzqvanst.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wsekxaeq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2atoctpgu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2einwjkgg.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ndxnakmf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2yllwoqhs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kapagapd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2knhsmytg.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2gsfwxiyv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tjfvroxt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dgebhkzz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2daynelbs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2innvdsoz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hqmxlkoz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fthaobdd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bzboeemp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lwcamcxk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2hkptrikn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gamdwwuc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uukbuzuf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahqlpsov.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dokrvukg.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnrtydbr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2rpsepdbi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2enxhwele.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2mcfsdanl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jckmxehe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tramcqtv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2smhgiciy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ndsmjmpu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gygwssdv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tywbvesk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ylcrgatm.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nlqdooxo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2lcliehlc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ihwozfmb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjfywuu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2odvieput.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2bdnfcsfd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ilshczes.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2vowpwolz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afylpxgd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2dboycjcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evcdkexv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2esbwxvnl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2oxnfozff.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qezjdwhs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hnpsrhwx.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ukibnvjv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2zqhugnzv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vamscdrs.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qajhqdfr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2aqwdxdap.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2msxbvgkm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2onnldthc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2njfzppec.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2tgnxavur.html

);
来源：http://www.52xcode.cn/Article/details/gt2yakappsn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2wkuqcnox.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2osipikit.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2lmukjuvg.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2kzlfjkpc.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2atnnvznn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rwllrwiu.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2rpweftcn.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2klzywejr.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2mmxxklqw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2dhufvigp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ewonhgiz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wqqnumqr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2oczabkye.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gbandanw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2sebupsmz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2azukrtcp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vugpqkee.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xkztaygu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2zjghomzd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ibyxsnrg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2vvnwwvmf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2gkvggqjp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2efvvgvew.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2wcomekkb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2mruvdwaf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bzksxupe.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2engtjnov.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nazrfsjl.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2pkwvcmwo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tkmgsnie.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qaskdfrj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rgdgpetp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2laxfbphz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2meaexrhm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vfxwkvqo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dycuimfx.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2uajhcmci.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lpmvsasz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2bykjptob.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qxbyfgsv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2jzvryquj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xwbfocum.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rmbypsvu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2mlrglcpm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2pnxmovob.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rrlbxjfz.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2xelwpjhq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2cmrhzcqw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2umrfnjhn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skffthbp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bmojvipn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2igxgjnkr.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2neyxclnz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iblciqsu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kdxkwfdx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qgvyztrf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2rigfgbtf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pwzxgpoq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2essozppc.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2lyrpkmuu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hbybqqre.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2emkmohym.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lcdtoasi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2zzceerle.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ffkjimvr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2zsrafzcg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mqfebufc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ietcxtdu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxetppfd.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2fsjzjfrr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yuzjbwai.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2niupnyws.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rqvgontz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2awtzulom.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2npjbjylp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cjkprlnz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ddynhpnx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qhndbynq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jjvbladb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2qbaqohaz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2hfjyegnh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2plhsabek.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2cxiqjhfc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2oxlutgch.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mzfpzqor.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2idyuyjhs.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vmiistmp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2sdmnecda.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ezogkegz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nardxcxs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2bwskacqs.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mitjcmaw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2uhsmewbb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ifbdhqrc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ifsnyeaw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2bkpwslyi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jwjnvzpp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bxdgjlop.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2svpdwdcp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xrrhmfoc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jsrbmrfz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2qrlftiwv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2nmanthip.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2umngpqms.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2lflzexuv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ofkxtndv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mhziwags.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tupllttk.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2brvaweuo.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2weyzudfn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ybdnqvkj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2htsovrbv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fbmxqini.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2cqcjkpzb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jmtiqdun.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jewofayt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cejfajev.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ulmfcdfw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cpjwtccg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqgrnwvw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ibvbvhkw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cxgmgvgl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2teagnfuf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rddaljul.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2kgyqydjj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ufywdvyc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sgabiopo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2olvnvolw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hztsulzv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jjjxqwiw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zdwpbwxv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qeckcwpl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2lnizyibx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2yyshqjrq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lpmmdshx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2zvillfxs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xccylnqp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mvizndas.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ibhbwwes.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2cwgjzwzb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qpzvswfk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2uungihwf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2tgrdtorl.html


<!-- 参考信息 -->