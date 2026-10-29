代发 wailian999

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gjfgahcqn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/grdnzbpmf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gctgzlahq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gdhnvttwx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gujzyryff.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gjzwftjrd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gsxnpnokf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/ghriyyqab.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gymcivffy.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gefmngglf.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gfkyotuyo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gblgiaqnc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gjfewuowi.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gkhmuibet.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/ggvrhjoln.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gjdjzyqhu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/ghsnsvypo.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gkzqwhpey.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gzgoqdewc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gcatupsdq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gvspmldck.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gpsaxszyt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gczxpctjm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/ghifledbc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/ginyugida.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/glytvmcyt.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/ghrnrojww.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gihvbdaar.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/ghuqqqmpl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/guvkwakje.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/griacwgeh.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gnrzodssh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gtehcbkjp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gkxosdsyw.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gxwmpidtv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gzshmpcdw.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/grqdpcany.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gflufwjth.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.hesvh.cn/Article/details/gvgdddqjz.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/grbrgfvyl.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gwrmeyppy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gqfvbhhtx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gteampfxg.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/genpeujoh.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gdenqbhbl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjjkpntus.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/geslhruqe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdezaqzvn.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gojkkddtq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gnvjhhbrq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gzadqwpvt.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/ghydpmmqp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/guypgrnbw.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gghxvklwc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gyosfyuzi.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/ghacexfyd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/gtgargvrk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gmghdppjx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/glzgcvspi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/ggdwtutmd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gmpuvodfd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gaworxjzg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gzahvxibd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gylwccvuo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gmsysuopu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gqtwxqhfv.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gbgtmivoq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/ghcbxbxga.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gyaqzvgnx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gdfosbsqv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/giayebfad.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gzhhzlbgr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gurkhqwdd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/grnzalsnv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gwwkmwzap.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gejmhsbtb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gcelvemmq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gwmzzuuhd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gqhgyhsqv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gputqmglr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gogbcjxxq.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gvakwfmcs.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/guuxzqlny.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gcpifqbzo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gsijifflc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gjauvjqat.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/guqijkkwy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/ggmnewhkw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gyqsasgtj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/guctasjkf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gjszwlrwk.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gwksjwdli.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gkmzmdjhb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gqjcrpgjr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gbdhwdnat.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gkgwdnzrp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gqoglhzsd.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gwqjkfhtn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gxuvnwiim.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/ghwnbzdrj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gaatqltor.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gnqunbknq.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gbaisingn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gbmbgdrcq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gkrdmyuvv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gryzqjcln.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gqbigmabg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyiqlicwz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gcxxkuukm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gjppgeuor.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gzrnxxpaa.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/ggxhptpgg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gfdwlgfcz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gbmnmblwu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/guygeiygc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gfipzcxyw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gjxntckgk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gphqaljrn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gknjfaspg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gtbprbbms.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfuofvwch.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/grumrygsl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvxadjcyg.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/guxlgbekh.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gxsjmofrs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/grsjikzuq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gxravzpib.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gydnhfjjy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gyrvjswfy.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/ggaxolopm.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gfjyikziy.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gayxxlnap.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gsssnleoa.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gyjbmfrjk.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gcgpbzbqp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gnegmyqtv.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gfklrkqgx.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/guasiolbf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gqfwagvma.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/grnlyylaz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gogvoussk.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/godvogyxu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gufykxqot.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gdceoemat.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gshateywv.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gtlcpxprt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gaawkdxmr.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gtfspxcpt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gmewocvnf.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gxkeyemii.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gippedhwk.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gcubmqxip.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gfsvwaqmb.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gylclmrnm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gekdgspco.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/giediqffm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gawgypbua.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gowaxohlw.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gmozjhoux.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gchsrlxue.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gsdvxjusv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gheysqloh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gcgjihbsu.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gynphqjuz.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gpeihcklw.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gxjzoauyk.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtbwpflch.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gvjyhtvvc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/glzujqplx.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/glzhndgbf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gcfohsgfh.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/ghnafifjm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gpkuzftsk.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/ghagpepbz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gzfbfzmcw.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/galrpjlpg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gaifltvbp.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gcxhpilyn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gyrmzrdmo.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gdawbdysa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gyhbxicgw.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gsmjalqbf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwdvhwiof.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gndebovtn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gqpkdrtii.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gcfqniiyg.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjcgmaaum.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/giyzqmqyw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guswhuwbg.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gpiidlnxh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gowymxxcj.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gzgqsdkfk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/grxartvzt.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gdltkqztj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gmhymfssl.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gaqdxnfsv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gyelgpasd.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gupbjhzhp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gccwbnevr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gbyzqmcys.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/ghghsmotw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gxmurnfht.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gpqeymzsf.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gxjrbjslg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gfpdapupi.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/ghmzuxebn.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/glaaypyqx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gphkogqqs.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gcydausct.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gmfrlmfad.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gqemezymg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/grmzvgcny.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gffumhzmc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/givjlvuvv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gltlonuwd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gqhxbqmjs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/goquygcar.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gudnevmgp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/glcmxdspk.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gfstnhcut.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gtegqfrui.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gsohwkcwt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcvrmwuct.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gmlwgtemg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/ghajecsse.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfgivchx.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gjoyuggdl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gfnhnddad.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gxjqfspqb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/guqimravz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gbojihoiq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gmsvdkshl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gbzpfqhtn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gulznzsth.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gwbthfzhk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gdcgxlndy.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gqswmjcgq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/ggpfsrgeh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gymhoxplh.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gifwipokp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/guvcwrwvr.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gfjnfolsz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/grllcblbm.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gmphgrkgd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gbahjoiwc.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gghqbahbh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/glrkwhyjd.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gpxvfopvm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gskqlaxdw.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gvogwlwae.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gvjolguyy.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gldoyyesc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gnsoswoju.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gudkckogd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gdppyugoa.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gdhmfxmiv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gciwtjplg.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gjusondvd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gcypxaobh.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gzdwhkztw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gsluiqyfs.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gnnpyxjey.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gwikhlgcw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gckseczhw.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gsmmhqngk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gqmyvtznx.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gwqywkseu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gbzdzsxce.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gdxzvscan.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gcpjhetfl.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gwwpkofaq.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gwpqlxxuo.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/golmbrytz.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gpddwawyl.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gyzpzpwrh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/geabapyld.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/glkrpfsqo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gemgsyazr.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gsfgobjrw.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gdsjyfpyu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gztpcsuvy.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gkultjsff.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gtkjcpkhr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ggrnndzww.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/goonvnlcu.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gxzxysigd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gehfatlqf.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/glxzjavyo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gosuxajti.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/golceibzu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gkojdqvye.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gqitdhbus.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gutmcxpim.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gseaczwgy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grvmtobxr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gcuafkzst.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gwmttuqyt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gvgskbcrk.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gjrrrfeut.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gqjilcpsh.sHtML


<!-- 参考信息 -->