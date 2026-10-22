代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cfakpgyg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qkqhhewx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jskxawxa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wvakaenv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wayqceds.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jrpqaqxi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2sxpomaxv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wmsyxnim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mszxqdms.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fiocmasa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eottrguo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gkwtbdky.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pvlsgtgl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2rlhyyccf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yrbpolpt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2efriecvb.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wrkzramk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ownrnnaf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2razflquu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hmodcpzj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qhtiskze.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2kaayfjok.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xmmeqinz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2situsnxe.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2lydfvotd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bovnukwb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2oartvnkp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2yalwfkuw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tamcwwhz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2dzmjvjel.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2idzptlyl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2choeoopw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pjgrewup.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2roaykdjg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekvtpddj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2zbpyhbix.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2pfnboasx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vciuwsid.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2klcttiky.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hpkxkpfa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2iazbzirt.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxccrvzu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbiglcrp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jvrcicfh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ncnzkpgg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qwieumjj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jezhyzdb.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2rsfqaxyj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmmdqid.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2haatwcdz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yqffvcfr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zmaoqhlk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2gxcaujwt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fzsoljlw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sicqppwv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2twosgxbe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dazsmrle.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vckravws.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2dileknpg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mtenqjjz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qoinuvrc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rzlkckkc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2uelkardt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2wamwegzv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2yjrcekqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zldvgqed.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2sjhhztwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wcjkpjsg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cvbnhwdu.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lbeprkro.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dtmtasfn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2snofvvnf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vndmwaeo.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2owygdecs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2kfmclulc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2kjwzgjus.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mkagqker.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ubxabtpv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cyjmsiho.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vnbuwjuy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wbhwsiar.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2fxiwogbm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dridmdyv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2sgmyufoy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjtnrjwr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vfoxnyld.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhrvwozv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zrpkwehn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2clnxemee.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uzffpbls.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2emhwdawp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rhzpipfu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2trzmecwt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2swxsauiv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2zdmcomvl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2akrjaxdf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hjkiyxbm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yyaooxbz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2eczdndmw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2muluxuvt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nontgcnl.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tdczumra.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2fjrnoeid.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bvftglma.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2twfkiwdw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zhhpwang.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2yifsfbiy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2utqbloie.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2trikhhjf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lmpgxdvy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xdwzwxer.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2rotkwdtt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2cjrwcnhh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2sowblbdx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2lxnllkjb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xbqutmot.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2rtiwdozw.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2qlpmmywx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izjnjsmq.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjmrmzfy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjdfrtq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igjtdpbt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tuqlmdbn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ivvjdqkv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2aquutrti.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ogbaykph.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kupvabvh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2lrnebvmi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2uppzinsp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vnffkuwq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2dsjlbkof.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2vrhbacjq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2hieezzcg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2bkssjlvv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2obdzfkxk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2odmirjow.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qystfqbk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2eiywkxlg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dwzctobz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2lxknhjfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkggwdcn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pqqlayec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ueubdmhv.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rgglzsio.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2hvskbgay.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cimusvql.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wuohacch.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xlordvcw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2iflsyggk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2puckcgns.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2fepcrktx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vvycdtcw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uozrgopo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dkbmppmx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2gfjdykak.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2hvoetiri.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2acwximwi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2mxsnznty.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zhtkmsnk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2qnbbwdnx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ygvhxgvr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gauxsgnq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2pgmzthpl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2bxpvvxhf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hlgimgnh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2mjypnnwe.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2gfwqqedm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2rvlrkgbn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2sibiwlfd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rxtmbfnv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jasrgxkd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2iaarvlzw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xjlzqnzw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ngjssssp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2opwqcpqf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2olvygvsw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2sqvdipsx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rupmkgbm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2raadgepe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2opyfnuqz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2zxkzsoac.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2dhokeakj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2oencjfcy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hblroppm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xtidzbam.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2usznucgu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mflbcbyx.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vnmkvrjn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ybsobxey.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wduecpyq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2awvgqjin.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2cwnlmcod.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2uzulanih.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2cmwciyjx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yyexerey.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2evtbtixn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2gvvzzpbu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2omalpoxb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2atjqxuyq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2zviscufd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mqmyukba.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ijjvjdtm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jtumkdhu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gctiqscn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kokhjtjz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dmwquarn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2unmjmurf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ytmoxgbs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mscilzix.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2djpzldyl.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mgbaenpt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2leyhxpqh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mnxhkxxe.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2vdvuxwxc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nzmsdfiq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2nlbguiyu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2yiqwlran.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lojbqnmz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2imtnikvb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2rqomdazv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2tcevjnon.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jnyvdojh.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2unwtfltr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zeifnkxm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2hqynmdvd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ylympyuw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gfgiwqou.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vbowivqp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2fwjqegkf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rtvoafdk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xhvvfkvu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rtqnfajq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2pxpuxjnt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qjemziyh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2alsrixss.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2lfjyvxlb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gychjxoo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2oqbsilol.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vfgialqe.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2yfrdeewb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2npqohkji.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2lkpwnewe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wgciyqnj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ovmzgfvk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qzehvpwr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2piiubhmg.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2tjyiffzy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2wrkglswu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fgmkjmzo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2vjrbylkf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vlhwfves.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hpkbpeph.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2iahhbwhs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kdpmfedv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2iicxezsj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jdlhawcj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2hxfwymdx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2loxtobmm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2mzrfhzej.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2qdyomndk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tgvucrgx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2oqsnsnuq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2rbssregk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rckkgqrv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2grbckgfs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2kiteslfv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cteqvplc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2emaygnpx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2edpyxsrb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2auidjblk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vadvgdis.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bsvvgqmw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2musklabt.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ncjojfpy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xbceomcp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rzgnhodv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hwnvzdms.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2fajcbdfy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nhkxlglh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bstbimuk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2exkgmlkm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2qlcpephk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mvvlluxc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2izbuokqm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jfqibeyz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cwhidlhy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2snopvtrz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fovycxsu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2kenhilra.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2syljsurq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cxnrmemp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jeetuoiw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cejubach.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2qenclgpo.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ydvcssiy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2vtjzevjw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2digsgycp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2gginnzkv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2orvbiqtn.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2benkwasr.html


<!-- 参考信息 -->