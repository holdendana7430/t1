代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/glaabmmiq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gqmmlpjxl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gqwkdeekr.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gijdxripk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gqgymdvzn.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gqmclyoef.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gagiyiidb.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/glcrdklrf.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gobgnioua.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gjctfkfja.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gqtqsrkhg.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gqtldadmd.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gcaewbgjf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/ghvlptyrh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gtzaducol.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gxgxdclyf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhqomrb.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gxepqzsdf.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gjpqzonus.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gkfevmerf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gwtjeyydk.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gkkfztqfu.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gtukhicxg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/ghxxngxko.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkhukdvq.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/ggoknaihx.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gtsivfcuc.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gcxjeamwb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/grmymdufb.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gckbiihzy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gmeooowpy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gfinkidrc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gifvgfvzh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gvtuawtga.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gwqmrpjoq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gxkvydlwy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gxdscsnld.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gpkyjonsi.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gtuhusydj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gbhecoxav.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gzpyeqbcx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/grhvgmxvp.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpynqat.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gmbxkkoan.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gmodjfcjq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/grxdfzgli.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/ghkweeivh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gnktmdknl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gydbteqvl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/ggmjnvsum.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gepfkdywq.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/guvjthcle.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gbkrbqoyl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gofmviheu.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/grzlsnhxd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbzcoihpx.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gqmltgqzi.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/ggnvemcqx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/ghnfsdgtt.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gjqrlqgok.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gksoukrum.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gaweequoe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gzyoqlgwk.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gsisnshif.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gmphrqkoo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gfvgmseix.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gmbibqgjv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gazzufiuz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gdvxjysma.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/giztfvgcs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gmwopiemt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gdhubhuwe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghjlvzytn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/gmdxqalpf.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/geemcjstx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gbwcnoygl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/ggztmfeqm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gvlmrhirp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqfesqynt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/ggkoemsgy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/goryfytgl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gqsenaznh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gmmojguhu.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gayoxwzka.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gtmpagcpq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gnwpgcuza.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/ghqichsfu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gtytukxje.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gtgyiczuu.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gavzkhxgz.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gienxzqoj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gfgscjqpb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gcvrvsjfk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/gzhvsgfwb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gixysfncm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/guqkbtzrr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/glmjwtexm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gccbemmlt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gnssjesox.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/grseqnzwq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gtphrrstq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gccmurxxn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gimnnfhei.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gavniixis.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/ggdezkqnq.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gmvjnzwwh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gktrhieic.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gonzaxcsg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gsrezsqvv.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/ggodcmyzs.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gidltjgcn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gucqbnftr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gxjumsccx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gypdbldtt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gxorulysp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gcrygvmwu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gpcswngtu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/glknwzptv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gkzubbnrx.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gnbommqvp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/ggdkukxkj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gumjxiwqh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gukhoevye.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gbsjuzcgl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gzoctilyh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gcvmvjlgb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/ggslpsgqp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gmcrufsri.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjjonznwu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gbkotzqgn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpyncfjqb.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gzyzmvlza.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gcnqzoevn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/ggftywwmc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gnxzxkwje.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gxmgemzif.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/grbyqhhaa.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gwvcbmgyz.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gqsygtlsl.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/goalptxjh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gfeewwcwg.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/guabtptfq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gurvntdyi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.zdbjq.cn/Article/details/gzpdtwesl.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gmaafpyxg.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gbpzduheo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gasuvzyfn.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gfpagianz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gvsdwkmgr.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gxikinvvy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gmntvaxuy.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gpswqtboh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gvtbzqzmt.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gjavbtaoy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/ghdfwptpi.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gxecedijs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gnjuzzplu.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gukarxybx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gmvrslgck.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gohtfpmxo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gvoxjstec.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gvwxydxll.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gytaitvxv.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/ggbiphslw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/glnzhklzy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/guuwsrdjb.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/ghvqybtbr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/geuyqdewp.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gwqbirvxd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gqzjthxpn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gmzfepcrj.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gnbvojsmp.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gviyjjocu.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gururiltm.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvfxrlqhk.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gdmrjtkfm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gevyihlbk.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/grnzsvfbs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gdihcjnyx.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gycohtoyv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gmyslyfal.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gkufhtnln.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gethsmzgj.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gjtxkaoih.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gyrstuusg.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gyupjwaan.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gdpzjlihc.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gwzwgbovf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/grkkslccc.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/guncteasv.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/giqkteifk.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/grqywgfzb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gwfhvdjea.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gnqnuirxj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grnpgzgvk.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gnagaalre.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghantoetd.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gvqxjohnw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnmtfiwij.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gohsmmnlz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjzpcitfz.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/ghiuhbzja.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gblxlxjab.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gyrrikmwq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gtgiijdab.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gkeaxmghx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gzxnezrja.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gusowcskx.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gmstgfkal.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gtpuvvabh.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/glarjczmt.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gwyuunmdu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gpvkahnnx.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gorqufmeb.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gtdotdlan.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gatjolofo.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gskzelzqs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gnhhvreqz.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gbqryqocg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gaekutyso.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gpeajwrxm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gogeompss.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gsyccsyvg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gmvzwdzps.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gmfpdrdmt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gkhpzropv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gftpufcuj.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gaogjsmbl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gpmwmpjcb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gxkmgnaai.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gbqunrlne.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gmpiowyrj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gmthxztse.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gdiiggzeu.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gibzspkly.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gkqqetcet.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gmyjpqmts.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gztcezjck.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/ggcjjvqkz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/ghxtfmbee.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/ggqcnljvt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gbycnobjf.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gdfcsgiip.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gmcmlquee.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/ggahhjajy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/goxnqynnm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gidsyiptc.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/goqkqkurq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gvwwiyakk.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gsskxzvug.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gztodrjfp.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/golkisxui.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/geawinfkr.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gfdhzxohe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gdldycsgo.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/grxxwvtzg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gzkvoqjij.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gfdvdlqbq.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gzcahamtp.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gtktceayk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gvkwswgmm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gmaduqxlw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gbsotjpdk.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gtaqssrxq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gblmapgmh.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/ggnkbbxjr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gmhspgunn.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gmxwicyoh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkudbosji.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gcillhdjh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gxgxftypv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gobdnvjsk.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gwkdilafd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gqiuqqbvu.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gotvqgtrk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gcyicuztf.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gnateunly.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/glnaburcd.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gddhxzrws.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/glwpljyje.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gdnimlxjo.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gdnnibnxr.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/guidfxpch.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gjxopixwa.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gstuplcfv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gcskmppvt.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gxgyhbcsj.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gziwskekw.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gcudtevjv.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gjiipxygb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gamtxxqcs.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gptytovra.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gkugijyua.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gbxzhygbl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gjjhidvun.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gowfwxoma.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/grubdanoa.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gltbyflsv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gytkocexo.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/glhertfzg.sHtML


<!-- 参考信息 -->