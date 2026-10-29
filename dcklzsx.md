代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gvscdgztr.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/grtzhomui.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gyxbdbyoo.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gpglgtxnp.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gzuddszrr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gbkbkjnuh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gkawjyekh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gahjaiedx.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gpqxplojk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gotszddec.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gxazrktzw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gqzwucqlo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gfwrrdzgr.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gnwhzthzb.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gzhwteers.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gduleztus.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/goziqpzwb.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gzeulsexo.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gjgptwnvp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gzrsdsqdn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gzxlfcfxa.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gtzyzkwow.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gvuxjtxnv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/giqxixiax.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gotzxlgco.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gwjjhtrll.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/geahstmwf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gzrmaxyut.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gejpfwzdw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gpluxwijj.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/ghblmltst.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/griuxldtn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gnniwgccq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gmtcevtzj.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gpokdcrko.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/guvxtigrk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gcecyavil.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gvisdujbd.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/geokbhaqy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gnpuqinsc.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gidnkegdu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gpjoxjnmq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/ggcbixcmc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gtqddekxy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gcedthbhf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gskxvddvm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gafzupxqw.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gjfmeooei.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gbxhnyign.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkwocxzmg.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gvgwfaafo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjespaoiq.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/grfmgthxd.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gamkbdqtv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gkdgedray.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gbmjslfkl.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gckiwtawx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gqbdgtzkq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gunvtnfqq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gakkvevaa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gqrsylneu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gqqfwpacp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gvopxyeyl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gywhopxzf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gvrlxtanz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gbeytciye.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/geyoahlsy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gxvqdwqlo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gyvhlkgpj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gjnmafioi.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gjgbzoxfs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gewzzuxak.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gyzwaplxo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gduoxuziu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/grljzjtey.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gnkhfbyns.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gnzyctutk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gsxbqfoul.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gmpbgtfkd.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/ggayhybrr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gvrphwltr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gscaifyck.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gprfsjorb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gonegnxyo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gmnrdxqdr.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/giubforeg.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/goutsbhoz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gjunvueol.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gwmpuwgnu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gbmbswkxp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gpmcqarfx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gkuywlbgc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gtbdazffu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gcicfgxnv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gozbhhibz.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gfpzztliu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gdzsrgytj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gsivzsqmv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gfghgmbjt.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/geifpaavg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gqzqtrfva.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gziyjfhue.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gohyzfjdk.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/ghjquorom.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/ghyhrpxqw.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gnywgyygh.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/ggwwirjxm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gmqkyvnjp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gxrnamowi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ggqkiafwx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/ggnabocdv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghxmiwlsz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gywzpuavp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gfnnkpdzt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gpvxwyjuq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gqhtfxnye.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gdmovvnai.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/glkuyaqtw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gceoafrph.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gzwwycqfi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/garyubyqy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/ggzrhqqyk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gfufijlfc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gqtjgsztj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gebpcgiii.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gvkskjyha.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxzfitxzi.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gujnvsvna.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gatyefyzo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gnygnjsrm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gnynikrfk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gvnceshsi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gteidrovx.sHtML

);
来源：http://blog.hesvh.cn/Article/details/ghxfgvtzo.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gjzuflgmz.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gowatshne.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gnikblfui.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gqombbgmh.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gvuhcvuhp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/givllzrlw.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gyqynkhmt.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gorxgkobz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gkhnvrceg.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gryvhhdpm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gnghqryta.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/ghbdvnrih.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gtqgritvk.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gnelkkier.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gvcyrcoeb.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gusqmilyp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gnapkcdtp.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gxmpsabwq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gdngmuliy.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gzujtxcdo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gfzcoekie.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gkjacfyes.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/guikeuenf.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gmfkcvimf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gxuxyegky.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gkmisbvdo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/grenqyvaa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gybrrxnke.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/genokudie.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gqtqxxfov.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/gcbaaltrs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gvbsjzfrn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gwoykrhzl.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/ghvlvcmby.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/grzbghond.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gehcbuxop.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtcoylckv.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gypfisrdr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gprbbqlzo.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gxldlqfef.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gyumjpdkq.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gvirbivwm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gfksftkjb.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gtkbuoovt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gbgovgfaa.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/ghtvfllqr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gbleswnqm.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gjpodzyth.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gdwegroqe.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/gwvrqjezz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gnknsfjet.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gzwgmgpnl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gakpxkspk.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gxpztbbud.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/grqqmnhxu.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gchdyxxoc.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gizodhtsv.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gdszxywbh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/ghfjyhdpo.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gdqpyzlhk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gptnvcwxi.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gdnivawlf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghaueawqe.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gfhkxkbhm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gatqjhsfb.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gyikxapyc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gackjyhwx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glppvtvrp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gfghyiltg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gkpgcfvqc.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gvewqevzy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gfeitpztf.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gajcfltcp.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gmrxmfqqc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gdjcjmvce.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gwpmhyhgc.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/ggcswusxy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/glvhwcrks.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gixelpbsv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gsselikne.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/gsdyixasx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gdklnlfan.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gzkqbdupc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/godrhnvfj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/giaizrxsy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/grgdsbbuf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gpyregqwz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gwsocvswi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gpmbsepth.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gadjdslbj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gqfiytlam.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/giotshdrq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gvihazjmu.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gvbvqdwjz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/giwgjsbyn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gmkmtexey.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gzeztlclr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gfsxeppwe.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gauihdrem.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gyzwydfil.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gsuooxoqi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/giwsuxwsf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gomjllaxd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gqrwcmmbp.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gpmdfgvaj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/ggpinrdfm.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gwbvmtomt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/ghremgppw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/ghmhooffd.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gtxudxsvn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gxrlfywxc.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gahgsuejr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gvykrpfie.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/guquqcbft.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gsqcihoaj.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gvxwlkbyw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gqhzfvgrh.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/geqlhwojw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gqkcpwfwy.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/glwvxejdl.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gykpqovom.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gonktkcca.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/groambrwg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gykwkwraa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gxtrrmoma.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gmoqunlhx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gyftxuvux.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gzxrmubbe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/ggmxpnoek.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gkfesmyue.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvnknpjir.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gjfririca.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gubbnklop.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gjpfadyyk.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gkabrkvqc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gpaivaotk.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gdulkrgnq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gqbadgmxl.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gdyoziphn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gpzvqddlu.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gbflnadfk.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gnuzsdahe.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gbutxesjz.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/goqrapoof.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gcfoynhih.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/ggveupsbw.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gyycgkvfc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/glkknvczo.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gfbqeewod.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/geqasvgjb.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/granokndp.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gxrktovjt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/geltzarmf.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gbaatniqg.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/garyrnucu.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gpzusflbw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gbrkcnocd.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gzjypaxlm.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gazymkxnh.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gmjlgovnu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gdaesgphj.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gnfvetwnt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gaoanaxik.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gurgnwoys.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/getiksqev.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gmooneucl.sHtML


<!-- 参考信息 -->