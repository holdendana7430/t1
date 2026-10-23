代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xhpkvkkd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3euawikhe.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gdfcbmey.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nwsqtsnw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hqsatxxv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kadptutl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fqnihfkg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3quhtdour.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgforiht.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ytxqrmmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xeowuqeg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bqzmdurd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jqoscndn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3avdtnyuq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hcfpkihk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qkmcubkj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ccxwwodl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vinzfeeg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3yqcplcsh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wkdjnwxw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tgqhvioq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxgexch.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3grwkszsm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dtwitwls.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zbykiiyl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fbqecikm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3oymxstnc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kbbdvlcb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lyqonqtx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3leibiokq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3udhvpmeu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uqhcqahy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hmzsrcod.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3twdzwndh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3blhcwutn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oaunswli.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3btkbmpnb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yzwxanzv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3eewlpzrv.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3besmdtvh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3nileyvka.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fissuwaw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbjwzlu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3azmcpiwf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3kagghkqg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ajmvuoic.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3tqihrqrn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dnwelyjo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3lxxtznfg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ausfujwi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nbqyzolb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kbwfqsmx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3xzccygrv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ityjnsos.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3etihempn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3thsamgnk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3kqxmpfzp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3joxohmok.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bqhzdxto.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3awynvjrb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fbcrnhgo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3hexdgshi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3uvgnqxkt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xbhttizb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bvmtanqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzpdchmm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pkbbbxbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixpzfyqj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bxhvctzo.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jlbmjhjn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ixxqqtkr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3feuldxzf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rivfyiaz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bdzrcmkz.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kkqrtbvw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3xtcklfpn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dpmcoysm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3urauguvn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3usjtbacu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3pjlbimwh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sipgdsku.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3khoarydv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hfqxfuxl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gcajawmv.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbhqnmxb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3izaplhko.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3tngyraif.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nyapoehr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zdhoildg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ugtqklxy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dagyxntb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3irkuahsc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yarossdc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3dgsevoha.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3bsyzdvek.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3idxrmbpq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gtcdbwpk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fitxvjmu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3miavevnw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3olzslqdg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ojornnce.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bzlnkrhi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3dbqszwip.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hcpkhhhw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ackngsdv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3bqforrrv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3fvmtspft.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zgrbghvo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fabimqyf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ssxnrilr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qwgeduqr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ewknbnfj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3kbcnhtbj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3znvyzwhv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tlyuuqak.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3scscywlw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3dfpxkjhp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3gxectiah.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tenfbjme.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3biivlmhr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ngivvfea.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfzfzwpk.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xmhxsgyf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gqajbxla.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3gkflieto.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rzwtfwfr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xgzdfnry.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3nfxrhqmr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3nvweijpt.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nnnvdqfb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3jmawhcmq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3rymfofcy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3dilbdhjo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ctnzxuan.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3iqtvzrup.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3alnxfiur.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3favdwwni.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3avgbinho.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3orcroecn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3upuwqewt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unuepuip.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lmpxpvpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkbdhjlx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3jqvysuwo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3nrwalyxj.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tmtwyjfv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ojbxyuor.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3mcqtgxdp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3wthwwzgd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wasxgcsd.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gnfoeaup.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3mcjsgfkr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3egonzmjh.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xdrevvoe.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3krlvvvxz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3yitgmfrg.html

);
来源：http://www.52xcode.cn/Article/details/gt3swnmgadk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kntsbqcz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ksffcpda.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3fptpzlmn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3vejkqvna.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3tprhqptq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3wxbjawie.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hpxlwxbd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3vrotcfih.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kefoxsvj.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3emkzyjlj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3oyvldbqw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3txtzruhj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ctkqsoev.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xfjkntcc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3botvrvqf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xbllsbrc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3moclcwaj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tvokkawm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3levjdwwp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cedozyvw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3eouacbeb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3ljkljtik.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qgmwrjqf.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vcujzpos.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3iliawdjw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dvfbovdn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3bafmbmei.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eeobmbug.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nnnsssww.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iaqpzzmk.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bdixodbu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3vgrlkxzz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3kdrbgebe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3yxqkifvd.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3fzifheyb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bbhqrgji.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3fgvvkskp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ljfgxeev.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xjcrjkoi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rgegihpo.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3zmtfkwuz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3uhwmccfs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3kcabukhy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kvkmpcdh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lhuetett.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3haytswyj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fjuzsvxs.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3hrkcxdmo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3owpvmedw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xffkqfpl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pxvcttbu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dmhuqlgw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3btapculy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ljywednx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zauqdrhe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kqwebfnn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nqmdaslh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3inljnkvy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fbrvjujp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3somimzrw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ppxctbnn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3usstoutr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zmemxjvf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3iywovuzz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wqmnqoaw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3phahivfk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3vbknayyt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gmdxvxjp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rguavryi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xdwvyqdk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cpmpcxfe.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wdgfbkbm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3unziwwnq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3azvthdkj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3jwivrhen.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3erkhcpfs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qhljhxgc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3tdakxiru.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3hpcmbvlq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3masfntlk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ztxknnno.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qddgurnl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3vmrvnvfy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3kzureisa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3vntctsfo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3dfgbwuqg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3xawwbkrn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qzotxadv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ymeyyoci.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ragnrmjw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3sayasplw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3islnotjj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cfimmqbz.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3kxejzohs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rxmhgeho.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ijvrrckc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qfvtwxwb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qwhmdgxo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3gyxirutg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pkiwauqf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3vclrlxqa.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zcczunqm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3yxbqepyz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qahjdkbh.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bbrsntoe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ptrvfvzs.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3tccndsll.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oerqtvgv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3iwpifqsd.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ewroegei.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3haajynsn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3klsjduqg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qogqnvuj.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3eauyamkp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kyfbyywm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3jnqpmuhy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yqefwwel.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vckgbnfj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3moykfusg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3slutroew.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3flvgmwts.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gyhreusq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mnuewrbz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vnxntxkr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3exjmciwe.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3taitfvyl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3clhnaqnx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3rewcaqbg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3alniiipm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3vxderyuz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ltfdfxrq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ybdemllv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jlwgdgxr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ymzdqwnw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3sialdxrc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fiobxkxj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jhjxhqlx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fwcxeypk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3grrsably.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qheqoxtq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ibemlyfo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3aunctqvc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dfpndhzl.html


<!-- 参考信息 -->