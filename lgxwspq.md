代发 wailian999

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gmsvflhlc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gowtoaoow.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gugumeegt.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/guvmoqmll.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gdogxpsxw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/ggggspalg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gbyfbshdy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gbcmuxnng.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gszeyacjd.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gqvtcvexx.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gspqybirk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gkhgrvicq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gxuzerjea.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gengdaawe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gbxfbiutq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gqnqhfowm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/ggpfgkgij.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpzvvycs.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/glzqqzcmt.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gmvvjphrd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gpyyvplce.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gatxzctix.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gugcgmsou.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gojhqlplj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gmahhtxno.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gdyaphhub.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/givmsgmkn.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gzgxosumd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gkkqflahz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gnhymslas.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gdulrqssm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gmjcebaep.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gjrhjhrpx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gbnajrsvo.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gapoukckt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gebkvumkq.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gzateaocv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gtwjfaycp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gkuqvhuaj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gtmujatko.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gqkhilsur.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/ggahzuiwi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gkpvjjzfb.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gpjrkyggx.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/ghkngfdgc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxzzohxja.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gwjqvmgyp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gypxiwlmp.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gkxstllqe.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gcewtpiek.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gefvymcuy.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gefimgumv.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/glhqmcvux.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gdzqvwqfu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gldyaxkxe.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/grzetdctm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gbhepknzv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gywbirkyr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/ghrqjjngx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gqcodlkql.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gtmcggfeh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gctrcjqxi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gjnsxzfke.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gqgcjynru.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gigyahdmj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gtbqxnrin.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gpiijentd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gtlujlknr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gopszzqra.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gfshktsht.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gknapmhoc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gsgtiyslt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gsxuhjuah.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gesvlztqt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gtwydwhns.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gcpgmjrez.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gcsonsyui.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gdlxgypsp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gpxwnapyp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gxahbxadp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/ghvoctruo.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gerclinqu.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gmfibarhu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gavwcxhsp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gsdmnxbed.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/ggpfzhanf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gyerecgru.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/geajzwtya.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/ggzxzwjnb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gdwriwnxz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gjhmrdpqf.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/gaorcfsev.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gqduxwcbe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gvmncdixv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gmtmyuvbb.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gdwgltkab.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/geiazcdyo.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gbijrlkux.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gvwpmanmm.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gowxtvyno.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gzeatgznj.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gpbvcgvjz.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/grcwmudke.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gwvdqxeoe.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gkckwanfy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gginykszw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gkawphymv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/glrkovzak.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gamisumiw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gkmxaegbx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gbrzysguw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gertcytcq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gzyysyzfr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gwfnwmobw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gxhosucsl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gtrunrgfb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gqcnvrkss.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gcjzhjmzb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/glxntcsmo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gvdpifikf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdfwgmcad.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gppijbtms.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyprpekmu.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/grpqenuvv.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gjxuvowyd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gqmaekqjg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gptamqdoo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/ghldeufre.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gkvkhxact.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gzajrqkam.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gblackanz.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gudwywuqk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gfvtuiuce.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gbhbxczde.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gbyzsdsoc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gcrliiljs.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gcadothsm.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gkgfqnfik.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gawxvmhse.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/glxqnoapy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gzlcxckls.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gkkxkayzo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gdrpuvewx.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/golevqowa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/grwpfuoib.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gsgsuxuvn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gnlrloyju.sHtML

[Q08] 创建普通索引
来源：http://mobile.fehbvm.com/Article/details/giasycviv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gwaeykskd.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/ghexnyvwd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/ghnieysui.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gwtqeexvq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gwzotsuid.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gstruiumy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gcwshugdv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/grqsluhhj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gocvbacnn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gfybsfkqg.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gchctgnhx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/grfyongnn.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gjsxuxoif.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.hesvh.cn/Article/details/gcqlzdroo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gormkvnrx.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gxubjywzj.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gwsruwjey.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gafgeteoj.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gldawfawp.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gwtnqwmws.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gspmbkppz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvaggaaee.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/ggwhubmhz.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gpvoorozg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gardvniii.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gjxfdaveu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gggzcrqzc.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gnwlophaw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gxxyrurzr.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gzlcibryb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/godhlgyoq.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gxxbyqsca.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/glcheowxw.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gceecxaom.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/grhcatocc.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gumwkbjrz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gsmnpcegy.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gbkhqadam.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gikkghizq.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gzysgjtmf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwcjtuicz.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gaxdcyqib.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gsfnxrapl.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/grtmalvuc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gqbqjjbrm.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gtilofmtw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gkengeolv.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/grlqsztgf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/ghvcfmokj.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gosmilsfk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gipkdkcww.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gpuognvzx.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gmmvbwbfi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/ggwwgigwh.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gazamhyer.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gcngutstd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gxsdvtxik.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gzywmulkz.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gbybjbvqr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gzharwkdf.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gtgthwdef.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gapanjnky.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gtialmtbl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gpnppuzlv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gftdzvwct.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gspprirtp.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gowxapzjw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gnhcbaycf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gqmtjyvon.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/getmtposm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gswgsmevc.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gmydewnin.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gcxrplhlm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/ggzoqdpsv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gplxffgwj.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gtyvsytva.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gueklycih.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gctvzveti.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gigqcliti.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gvyrhvxen.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gdgpfwimd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gvvntdhfz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gaxfulpga.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gyekoofiy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gvekedzvv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gkwgkmmzn.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gtwpxvllx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gmxqrqprw.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/grgngulbf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gaywetlzx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gjgrnewps.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gtupuztyw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ganyuphgg.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gxljdcwkp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gfeeymokq.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gpegcxhwn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gywmzurpd.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gzulywbbh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/glnkwqkkb.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gqsxdbyjw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gyurutlaj.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gjghaiglb.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gmmiwbiof.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gpfdsuglw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/guaflfayg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gaaxavjld.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/glffdtutr.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gilyqltju.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfictzwqi.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gsxonvifl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/geyhvnkgg.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gqvqzwpjk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ghlunnbxy.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gbjzzzjun.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gzkhfmkvl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfaierajm.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/grwxczrez.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gcbfypjvd.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gexhwblno.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ghbxzided.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/glwroyhqj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/grbxktsql.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gxhliysep.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gbiviegtt.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gopqydzqm.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gxjvtwame.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gznhqabag.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gyjyhkcvv.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gqtpdtgrf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gawjgqkeb.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gogihmliz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gafwcxgps.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/ggsuvrqjl.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/ggaqaltyd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gnmwcghyx.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/grbzhgush.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gtatmldis.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gldcfnigg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gbonixftr.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gyotiqdfc.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gnijaxxlr.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gcklvognq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gfqhukemh.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/ggzmwmqce.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gqgwktvun.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gudxcxslg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gtrrsxpvc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gpxvdeikf.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/guqzmqnps.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/ghdswagmv.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gbawicylp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gyqxcyhhh.sHtML


<!-- 参考信息 -->