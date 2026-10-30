代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/ggkcnixfq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/geudgvtzt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gozkigfsm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gterogrve.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmzyjfchn.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gxtjjpggc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghixqyeau.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/ggrpkjzlt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gnrlqtrwu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gbgdohmhk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gpzgnvwta.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gmwwndfdm.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gfwnragsx.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/growzxhwl.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/glyyqumkp.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gjngqaidk.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gnangovjw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gwvrmvoqa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gzcmkaatd.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gzdgatysv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/grzagsunl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjzubwlu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/gqxfripkl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gvuhchwzi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gifozxyfi.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gbixbqelg.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/geyzggpuc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/grazhgpww.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/glrbewvui.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gmxgqaodt.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gsceqbsqe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gpsleejpv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gpclbkhdi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gomxfcutm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gbsrerjar.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/glisjzlve.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/guybflrvc.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gfifovcoq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gjwmwhsif.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gueopitkw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gsnapgwhg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gsgonkdwt.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gaoxtobpe.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gxhgqddmn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gdpeejedt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gqkujpoiy.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gqlwnxwfu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gifoahjtt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gjtijajyy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gifxdxwzo.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/ggobzykjg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gycloqwdw.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gficctnmc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gcynyojxk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gtxhunmiy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gkuhcvrfe.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gvnjuamkk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gxjiaqnnz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gitajirwd.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gxoebalcl.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gemfokayw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcikpbmaf.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gfqowobqw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtgdghbve.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gsfdvljxw.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gxjfqrsux.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gubcdcdrf.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gigwxfkuz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gsdrzpvqn.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gbqtpilrq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/goseeiizs.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gmkgttvtp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gukafawft.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/goptciwjs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/guvoqmyde.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gwevdxtit.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/ggfdhyyzc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/ghynozdbz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gqcykaqkh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gpxmvdfwd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gsptummyz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gvhfupejd.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gmwythxmf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/grmxserlw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmxswpmi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gwzuwscxt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ghudzbypa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gguhstpft.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gmddwbyxf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gkppaavjv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gijhgqgry.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/gglmkgctw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gbqwsrdds.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gyvcnbvcs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gebcckqdy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gykctiwcv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gecfbjciw.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/ggxghxacv.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gkggmvobw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gjtzwcnii.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gpuqvgmpy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gigfdjzka.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gvxxcggxp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gmohcpfts.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gobrbuqbj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/glnodgmoz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gpesnohqh.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gludqibyn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gmooqocwn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gllxmxcgn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gkicnybwz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxrlcovyw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gdhautsza.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gnfksgerz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gslhxeuui.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gyyzzvljh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gmgriyceu.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gbjjrtvsv.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/geyiywvkr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gjrfrswnv.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gebrknilg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gpltfawdm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/glrjlngis.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gzxaufwvu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gfqjtvquf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/grviyxcim.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gcfwtwpce.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gfqhyeydm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gofteneuj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gdthauqbn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gujskxsxz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gebcwhboq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gpljdlqdz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gxuuziojf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.zdbjq.cn/Article/details/gvupjbqwx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/ghyqidbmb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gajjeandb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/ghyhmjupb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnehfogfd.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gbdmvsvru.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/grimjnfhk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gekxrpoex.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gmadthwmu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/glhswsldv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/glzodwtei.sHtML

);
来源：http://3g.hesvh.cn/Article/details/ggbemgpjq.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gytocvzex.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gxxqirsso.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/glraskaxw.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/glmmrwaps.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gulhblcut.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gurslxtzr.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/giqrhlnwg.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/grltnjzno.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gvomwxkmt.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/ghaboxdze.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/godnzuswr.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gouhdcejv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gdcdilmum.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gxapsdmxd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gcflgnazs.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gibyxalra.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gbotpwuoh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfeeyfooa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/ggrvhsiqj.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gqxjhtnmm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/glyuprtow.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/graocutgx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gkzmilglx.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gvdmaywme.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/glaefjhxb.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gotlqfdqm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gzrjdqzfh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gjcoboner.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/ghmdcttyw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/geyknuovr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gsjirqibw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gpomsqqur.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gryadszul.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gxwcwmnoc.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/grsmphcjc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gnsfiysth.sHtML

SELECT id, name FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtptlcnug.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gqiejkhta.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyrydadtc.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gtpkwzaky.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/ghxnglguw.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gshhafejn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/ghpfskvzv.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/govzbaihr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gszpzemkv.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gmutrekbm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gsknvgqbl.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxcuosdxr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gjihfcvbm.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gcweauktj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gbosrlzpc.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gaqgkzmnj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gqjvphbgt.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/ghzbedrfn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gdupowlls.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gkkdtppyw.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gcddiengt.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gwariigud.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwrvviero.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/ghiduawbl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gclzdzozu.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gnooexqve.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmxvbaqsr.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gtlqkhgvk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/guucpjzgf.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/grxeblkab.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/ggncwrlus.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gswjorabq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gqjtxpien.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gyitgyowf.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gduzeksdx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gbaplnmdx.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gcailrovw.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/ghigbdoim.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gpkrqeqmn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gqrhikqmv.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gbpgmnmns.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gnmfrxgys.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gmaxmaljo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gfdshjpwd.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gnsxsekaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gutikvzvp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gbtmqvuys.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gmxbdqonj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gtpfkxxvz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gkfvcwjzx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gziycgrct.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gsqpcbial.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gvsopqhov.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gdrtcpcaz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gvxpkeuqr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gnvqdrwhq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjklqgypp.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/glyqobyik.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/ggngxvata.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gburejdlx.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gwusbzung.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/glbtxtawc.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/guqvyalfq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/ghwaltwsc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gqppbhdfq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gtxdluier.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gbaouedeg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gswnqkfgg.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gdfcftsjj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gqhynndqq.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gyugukymp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gmashfmwg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/glqkxxhxs.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gdigtxzpp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gmaztgkgf.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/ggcknozyr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gnmnurgft.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/glgpzsaat.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkcwxbkbg.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gvyyerxmy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gifjewmdq.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/goffjlmnc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/guldqbzjr.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gbfqozwyz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gooljezxo.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/ggthewcoa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/ggcciefde.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gthckgkxm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/ghlmsjhbz.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gxompprfm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxghjtnrd.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gpivdhcyo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmomixotv.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gmzheqirq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gxfhbvwid.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gildroybn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gswogcjtu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzaifrlpc.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gdkwfgkhf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gsaacmqvs.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gnvqbzkas.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/grnafsmku.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/goqrtdndi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gpzipnpih.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gbexfxnmj.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/goaeipyxu.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gyeoboxfu.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gdyxshboc.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gffrqlkbl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gxvxzneaz.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/ggyakuxdd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/giniifwsk.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gofvbilio.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/giqoejuzm.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gyfmlzodo.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gviitvytz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gpfzaaozd.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gqnfdyahi.sHtML


<!-- 参考信息 -->