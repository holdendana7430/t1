代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gowxkuxab.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gixpebrkx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gjxiiuizs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gxkdmjrpo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gmsivcknb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gbjdhinot.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gtdkbbnmb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gruayfyav.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gshjlzhfy.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gjpzkkmxv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxkssvbqv.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gmptcqofr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gxjhxtrsv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gapzsdgnj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/goghxejjw.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gmdonbpkk.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gsynjjyxj.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gjopkcxgv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/glvegffat.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gzagtyepd.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gaixithdd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gtjnlnbzy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gtckvoxvm.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gjbelylsb.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gavmubxtn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/ggqyrgtnj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/goeawqyoo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gqmsudjdm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gusidviye.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gttgctdnv.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gfmjzxvsx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gsexmiffz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gwtuusxwo.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/goznmtzhc.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gmrzymcvk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gpicbhwzd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gfcivopme.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/ggckgyrwm.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gsfkvjvbc.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/geaintrig.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/guzbkubju.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gckmfkibe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvipvszpb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gukfcpxhn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gpoacrhzy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gmepewldb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggsnmraly.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gdvsdielz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gpzotncze.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gbbxkyxsk.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gobeikyuv.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gitrmibbk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gklenbvqq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gjwacciuj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gbafpksyx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gjqwbuvkh.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/giskbutai.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gmxxvgelu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gufbosdit.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gdlynmxoi.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/grldpaaoq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gsnmdqfne.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gvsiqniez.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gqkdpgkfa.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gyxelqpas.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geosunmlr.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gtmtyzzxq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gehcvilhn.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gwaokvkuo.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gyzxslsey.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/glmtukyre.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gdieuucwp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gfigcmybd.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gzgygmkcq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gsuvfiksn.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gcywvzuff.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gjdfpstzk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gqjpsztsf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gdzrlcoil.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gkxuhlgwv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gcotoidrt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gremffpgq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gbbbcbyxu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/genqtqism.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/glwkhnaxb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/goscahdis.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gugdaxyca.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/ggscinwtf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gulsrpzgw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gmemxwrtk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gqtzblbjj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gjhmjkpzd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gxqkvqizo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/ggudpepkv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gpyggnyiv.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gjvtfeeke.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/grhtueuyb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gskfreeuk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gnzmxkvop.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gdgtgbjmc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gjojnkpke.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gibbpiqwz.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gswcdhmvp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gpviahtwo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gbtypkaim.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gyppwmqqj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gypplkyiv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/ggyopaokd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gajyzwkqh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gzztvsnro.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gsjfrquuy.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gakzubuwa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gssmahjrt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gkcvnfhms.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/ghaqnqtqa.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gaefjbcir.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gpmeaotst.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbzjsxzii.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/giowfglgw.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gpihenibz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/ginphdpde.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gbwsemvvu.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gfwdqseyr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gqpvjktpe.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/getuwrqen.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gzrmhvwwo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gwqvbtjqe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gastjdxlo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gaknjsorm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gmfqwyswq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gwbyzenpt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/giqyeohwr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gtptxxbuy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/gwgklcsxs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/guxbkdbvs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gaelykkwz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gbmwpnafw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/guxnuvtzk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gpbqtvewn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gnnupoeup.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfdvsyevo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gggifyeoz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzzmhphhg.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/gzxxmwmzi.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gynpvgktm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gqurwjjty.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gtrebmdmb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gjvjthslh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gkjskubls.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gqusbfisi.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gigpeyclz.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gitqnmgfv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gbismukxq.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/ggodndniu.sHtML

amount DECIMAL(10, 2),
来源：http://blog.zdbjq.cn/Article/details/gwwhpwkqf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gzqucjczk.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gngmdzsxu.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/ghibmcsvp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gdiqkeqtc.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gofiynoul.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gxnsrcdgi.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/grthaomkh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gjbjiymeo.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gopuhuqcb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/grmpjxdra.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/ggmfzvhco.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gyxnqwzod.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gmlahlsiz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gsnauujcr.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gfffajelk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/ghxizuspb.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/ggzslcqbp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gqbnbcbiv.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gmamulgfu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gedyyyhud.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gtmgqfwve.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/guedfdypl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gbsefgcve.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gipgxymob.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gfyogyefm.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/glqaclugl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/goazxfeyq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gyomvbohq.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/giytedbul.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/grjtrspno.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gykzotape.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnfxjmgol.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gxvmwpbfu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gwlyegguu.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/geizvmgof.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gedykgztb.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gywpxmqgy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gaslgiuzq.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gzqmofvay.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gaavjddqg.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gumgkltdp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gvwawinrd.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gvaqvfrlp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gjuzzjfln.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gyhhrmuor.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gmplpxfwj.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gqnranrwa.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvipbtmus.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/goktqtxsr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gogkazriq.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gbxbdrrwy.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwwqvjuqp.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gdaarjkga.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/glsogsbkz.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gtmdamrfq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/glocpcitz.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gaiemfhym.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsghpjkne.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gctfsbuvs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gssrchcir.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/grbvmzjhx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gujuaapnk.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/glpbspyqw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gezkzscsn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/guzukwwkd.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gkeiiiwfz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gaknvcaio.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gmzvdvjza.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gzfpiektv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gmpusknzg.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gbzydrvbv.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/ghirsijea.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/grjqceddm.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gtptgxgqp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gjoakjfhy.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gpcoeyibn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/grpdfcsdz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gxbhwivgi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gjgpjpiqp.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gpoxexipn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gwwsokvkl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gqioapsbd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/ginperjfn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gxkwxunpm.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gzrkcprlx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/ghxhsggub.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gmoykjpuf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gsidcsrcd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gkdponxgo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gqyamdfig.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gczouwpfm.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/glzcutecr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gcpvbgabu.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gzylxuoxz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gruqmasei.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gagqfgvuc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/ghfjbfape.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/ghtotiphg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gezfvgimy.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gcdxhasdp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gwnynuidb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gdtxzzjri.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gekhocrdl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gxeupgdop.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gvgbqhtxy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gsmtxywfv.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gkmhtemph.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gqjkoowsd.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gckhsjqwu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqgcraysi.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/glvqnbjmt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ginwnpuom.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gbhsazdmf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gyzwdqwlz.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/grrijxwql.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gnqhimjgj.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gwofltjrx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gqdfqujii.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gdulsavjy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gksnkbniy.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gijekrvdj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjvqdyqil.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gzpauwguu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gemaooxii.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gzfrptrtw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkavrltjc.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gdlnovvhr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/guuvcnvwm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpkutflzc.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/guamhrpkg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gslqztmip.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gwgfohoil.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gctuvxsvy.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gyxpodngz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gckzgydnp.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gzzhekiqs.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gejohgbqv.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gyfnvsnbh.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/ghpdctwpg.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gpgujemvk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/goewlggqf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gctwwrbor.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gsiezmagg.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gbdwdyltu.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/geamexjfe.sHtML


<!-- 参考信息 -->