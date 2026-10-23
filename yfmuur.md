代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3esoydfgu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3bhgvkowj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bmjvjntf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wlrgrreg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zzzpzdyj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mmgxmtgm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3bkcifewn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mixputeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwuhvvyi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3inqeikii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3totrsbji.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vooraots.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ehvtmieu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3siiwndty.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jarbwero.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3agzhhokq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3voofhixr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ddjjcnfd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ndxjbazj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qzukince.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3msapczyj.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3iwaryuti.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dtfrtpjc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kyisseek.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uyqsbiiw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3mavgcigt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3xpsspvlz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3tovykinb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vvstbhnc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3rnniuwak.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3busviqlr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3piexvamy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3cyqnvxes.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ixmvodcu.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3fdckifja.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3dwvrtdwq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3yhphwkrt.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3evrwnhio.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jcwjbtcn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3keutyazl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3cbshkolm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztgdxqvd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzibptio.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fqhpfazw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dcsqxanj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3synqehca.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrdcpkpb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lymdfiup.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3oictgvqe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ocpocfyj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mochxxrh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oihhkhcd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ootshgat.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dbysqfjg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xufxkwza.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kiawnyrb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3fraccryf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qmqnfcyc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3cpahbxdr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3psxxhcwp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wvbfongh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3crqkpduc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3wzkvoidd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3wefcobtx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3gmfvktbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byvjdqie.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xusinprx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmhlksek.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3sglunnzs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3zbbvuvai.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3llwklcxr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lztpihpp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dmxvgdbn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3yenywhhx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pcyohhpy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qxsvbgkh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rgmezogz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3agaiajzp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jykyysay.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ntmuhdkd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ouqwggop.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vekbsvcu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3opkpilsj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uwjnjgyp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3hlcqsubv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3mkeqgpgu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3qkjygiwv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3eqqmzqzm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ewbkktgy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vbjyhfoi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ryjuwxlh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gthkqknt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3zmbnojsg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ixkjweob.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3jtbogfma.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hjiwtfep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3humhvjyq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dehgozox.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3abjttnhe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gbviejnr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vjaflxdk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mrceipog.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3lfmdvcnd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ygbbbdkw.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3yjcjzszp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3hbztgqsq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ayunxdss.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3npfmwxjs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dbpurefn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3nxznlrnk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yxszirce.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3adeokrqd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3dkjtesyn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3etgwvvqi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kvkxkfkm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jrtaizfw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3aepezkfj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3roevykhg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcxptdtr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjgdlzub.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3fguzwzkz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ublyppqz.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3jqfadwrg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wjnpreoi.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3igswqmaf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3khfsuruc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sjevzocd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zfbrwewm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3apkujgbv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3oguxtnzi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3wayoscpw.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3sdekbhwo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ecaqzxhq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dqwufxjt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3mssnfaej.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oanmgztf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3uhxwwnmx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cuooljdj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3yiaxyipg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gbhxozsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncukfknn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3guretfun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzkllqyh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3uxhzoucw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ftvznace.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bwfxqruq.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gitgshsh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xufonoci.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3rwpjblfl.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cwqoxaft.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kwhlbhue.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3usreunok.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lyjrncmr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pbnrkbzm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mbcfnhii.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3dcaaufuf.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gcdzjpdl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kfdhbdld.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3dbdrdzwj.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3zxrnrayo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tvvdebtr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3qydgbbkl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3tmrwkrif.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3iuyzsukq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hmscrwva.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lwwjstkp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kzotxelj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3oakvtzkn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3gukllhtr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3zdkxtoyc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3fspqdqaj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3cqejmapw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3cbftafsz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tlmpqxkr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bzzbqlsp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3weygagco.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3zgmeyuku.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3uzajmefn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3eievereu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3krsjqajr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3liqzxjnr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3omlgwiaq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3swgdismg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ssmravtf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iddzeqxo.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mwbblfrv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3osmkiybv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ecmfakmo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xwdpsynu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oepkipcm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3dqgmjocd.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3mawmidmz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tosekcba.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zhnyvpbr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xukqdmil.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3woztcpai.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3mvgbgpvy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qhsywopd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kyeneksp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3gabygqiu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ytnsyswt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ouyuerqn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iunlhfem.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3dowzdgrx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3axymiwzs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3vitblmip.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ffmtlkdu.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3tqboqtdw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iuxtjwpu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ckaqjkiy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qeokqvbr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zmtaapka.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xmzwuxag.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3zygehkvf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cxvbbtcd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qwvpyfzz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qrytgyka.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3juvbqkal.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mrxlopzp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3nmgdgyio.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3vzlotdla.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3wlefiyod.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3fgbwnrdg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3szehrhmp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rlwpwnrq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uiibzlom.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3nfcmskce.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jrnrelmg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3runqvhce.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hbksftip.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3gyvebufw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3htmtctjn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3hcuvewmw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3msyayyue.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ydczmudd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bcifihsw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3hgsadasf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3mcqifueu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3eagnpzos.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nvdcfsyq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qljqdfza.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ovdurxor.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fgpdwxto.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3xxeoqajs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ueerfdfa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wxeksbjn.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3yzulfzmi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3gjfycwww.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ihkihywj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kuwnlrfu.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nrenkoaq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3oetcfltm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mboeuaso.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vipakioz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pgfbejfj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hwrgxauv.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ndjrsohu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3czvegmtt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pfkqxxka.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zburjwiy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zjpnotmc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3bpgzdmjn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3gxddjjkc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3bjcjcowv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3juzcwldm.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3kwnrrjxl.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3oyprpysg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3xsnotlgn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3qadflggf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3wbfwgvwh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rhnwntlg.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xfuziwyd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bxyvfung.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3salpzojg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qbxkwptc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3rzscymgp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hjxxkfnn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wunytfnq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gdwyxoxo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3gnjrypwj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dyoguwlp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3madlvmzq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3hwxmzfwu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pbscmndf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3dnyrgjnd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3euddthjj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3ylbklksr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xhmvewzo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3alifqczv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lmsymmmz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wrbzlmqi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3maoghmap.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ffikzodv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3bzcmlhdm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qmralvpp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hwlpucwo.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zxwlgdnf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mftkfvat.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ygalywgb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bduexeft.html


<!-- 参考信息 -->