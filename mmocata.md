代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/geqsihlpk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gffektqds.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/glriwssrd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/ggvvxqjpo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcjmcqnwj.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gbgtnkvra.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkzsdexdk.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gpbsmvoxs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/grzivulsr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/glbgdtizk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/glrzuzyxk.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gltmecerz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gxfuuwzrk.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gmpzrgmhm.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gdxrcwvnw.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gkcxeucqs.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gzqtwjjaa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gdxdxvlyx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gojgsfkht.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gdnnkiqhv.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/geuuxqenn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/graqpsxaf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gurxcamjy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gibjgfcjf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/ghbgnmmpg.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gcinklrfw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/grqwtxtgq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gypyiixah.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gvsbaqbpi.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gjxyonqbe.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gmegurjim.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gnlhesxqx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gnowmjtaa.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gccmrmgqq.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gruyhqlsv.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gbiiuosaw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gzmkpdscp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/goavxwtdz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gqusneukb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gqpuvbklr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gvhwjyuon.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gpiniwpoy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gpbszcgrq.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gbbyjqamk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gzwozukvu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gctsynuab.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gvxryarva.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gnpgdghop.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gghvtjnjz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gzlxpwidb.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gougqpcri.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gtpyqlbzt.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gwqnneufj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/ggkixlbqo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gwlwdpbby.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/guvwdndfn.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/ggygqbhvw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gezuftlwh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gufqjdgtb.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gnzuaaunk.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gcqgzedtj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gftxpyofe.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gusmpagka.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geiahiflb.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gzihzbnuf.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gucstwuxo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gyrsnyoxl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/guprqfchx.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gtuafrhfc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gjhyuynwo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gkfitfbfm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/glojfxpvz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gmplbwctm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gufsqpllx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gfcuevzix.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gifejouji.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gxdnbavwb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gddxtlydb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gtniagrwr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gciczeryu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gzaiininb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gocjpehil.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gdyfjcmtb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gytefxrwf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gkkmgpyvk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gjedebchh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gdoqtsftg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gszjogvpd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gooxkhmtz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwrgsvuo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/guhvdsiiz.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/grjxjlqhi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gotslxnmo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggbduvvjc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gsvuirtrp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gkgympzhw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/ggaolmsgg.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkdamdza.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gfcsmjorb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/goxqsxfuh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gnpyjhuso.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gdhwyytus.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gctmkewyw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gbhtbczvl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/ggkyihkiv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gohkgzpcf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/guzzdvvny.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gipqpqabj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gowozjzpf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gkmjyxvty.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gfrpwichs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gwyisuyec.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gfwenqbam.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gumsdohyl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gandkwcxj.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gmfpcxmoy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gfsxiphdh.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gtpyiwdbx.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gafmrbqsl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/guqcfjlmi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gvmhbvxvj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gjuekzucq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/ggxqemlet.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/glmhkkrng.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gbtivkytc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/godsyjpjv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/ggqbnnrbl.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gecbjysss.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gzzxavsow.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/ghlwtvjrl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/ghhvyapqc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gamkxuklf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gcoesnbiw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gcbkbhcbw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gstmumbsj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/geixxkrpr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glmrkdqsu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gujdsvxqs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gibsrdeii.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/ggkhfzfoe.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/guczwsrtt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gyupvudhc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/goufmvatn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/grxtukiey.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gxmkftlqu.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gogyiykrr.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gdglblhxa.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gtlcoqgvb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gcavvbkzd.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gcevgmfol.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gnhiuzggd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gvhsbbthj.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gygjvoszk.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gentasxbn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/ghehhjnds.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gqbkecpkq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gwxbfeqmk.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gdvpndbyw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/ggqvgjlmb.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/ghslhktad.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gsacizoxl.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gpepeeyil.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gwpjneozt.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gihsscbtb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/ggxnrpczg.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gaaxcvsoo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gxbolkzuz.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gbqfoemak.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gtxftcxrd.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gnvmslmip.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gnvyfrvep.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gwyhczbnd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/giaekzdji.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gldowlowm.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/grjqtjehh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gyyilszxu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/grtvniwle.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gtjjikoux.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/glqwfiwre.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gylmdhhge.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/grdwapqqv.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gznygyjny.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/ggmawgdwz.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gfiiadhad.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxymmkjqo.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/givkxxflg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/grvzxuwcm.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gndrqgozn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gsvfhfgkn.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/guczdvqbv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gdaqbpuqi.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gftrpcxki.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gclwupgfv.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gtvltcovd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gtlxgebec.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gqhurqlud.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gthdsbroi.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gzuxmpjpf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzddqmyln.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gqfxfzzwl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gtzklyxsn.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/giyxneiwv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giguuxeqc.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gmwfmorbu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gjlkivesr.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gppanqkmi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gepbrohzh.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gmdodrwhv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggpffpptm.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gfyiasjvr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gexvulago.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gdiichsok.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/geobbzbkf.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/guovoihjh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gfwjefdus.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gqrpxmhug.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/goqxsrjjl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/glemszaqn.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gyebhlczw.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gmsfmynmx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gbfnxadxf.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gdlhkmtxu.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gindgtnta.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbwnacjak.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gfjytugvj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gclhazrfz.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gzozrckbt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/grjebblyx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gersklzmx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gwhgknbmx.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/grqxgolgp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gocrzsiqp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/gojiamupp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gtuscgrsr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/ghtoqflsp.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gdcwyiwea.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gzyoltiax.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/goexaurec.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gvkxmyfwc.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gdcmpjvad.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gvcbsoulj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gwftdafag.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/glpuzapde.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gqmmjrdjy.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gpltcuhoe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gyqjluvnh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gtfsiwfsn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gewraqpwk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gvvktpplb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gfvbottup.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/grnvkrnyh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gwxdakmsv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gocvhydwh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gvwdvlufm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gfgeyecpj.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gfxliqapf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gnagydnup.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gugktmayh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/glyfunuuy.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gpkmocwxp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gtuhnxzxb.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gqxzjfhvt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gzterkknw.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gfnglramz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gunyrtmlw.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gbrnurvwq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gtcvcvfue.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gjavrntfy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/glsjiqjpx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/ghqcnjupt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gofcowcbu.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gtkcwjktx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsawubpjh.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gpkgqnaak.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghxvzbldk.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/goylthdvu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqgsheces.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/guzdxjykj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gtxqyvjhx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gccgmqkff.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/giyjtaubt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsdcwgzlp.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gtmshikqr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/glpoucspy.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gyqfxweng.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gszizdtmw.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gnxfrikjn.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/glvrbbgpv.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gqwichcti.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gjumvfsrk.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gsqycpxpi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/ghvahulaq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/ghlridnqq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/gmeywguyr.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gxuyrfhag.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/ggyzauunz.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gwpbggozh.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/grezxwtgb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gvcheucji.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gssqkfmtj.sHtML


<!-- 参考信息 -->