代发 wailian999

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gznhkgzff.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gltenlapt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gkzdmhnqq.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gjtcphqvl.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gvwewylwu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gzsepvnzl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/girysnzaq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gsiqjstic.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/grrdrkyic.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gstloglll.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/ggnrktsnd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gyurjxpne.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/ggfnqtoil.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gllulidqs.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gvjnnfquc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/givcugbyq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/guhuvdjqd.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/ghbkeoyaj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gqgvbxyyi.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gdsouvvzz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gdqfbkqzb.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gronohuns.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gddlrnicy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gcxaxflbr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/gsxkphhfb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/ghxtthule.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfukqxymh.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gvpwjjkvs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gbdapkwnz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/ghstkqsqx.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gsvmkwrxx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gcgeoqdao.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gudpnhleo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gdynlofkw.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gfnunmamc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/geypegkbd.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gnqahklew.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gvflfenev.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gceodrhzy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gugduzanx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ghmfhgepu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gdjvsavky.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gbexasljq.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gapitvnyb.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/goqabjlrt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxfuifbry.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/guaonumpq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqnrdcctl.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gsrjoxplx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/geeqtrnjz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gcwzypggz.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gejgypisc.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gelddueye.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gjqyfefej.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gzozjrgzg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gimontayp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/ggwslnhdm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gmzwhufhs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gnzwqhlgi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gzcdxldbp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/glbsfevmo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gwysiajin.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gkprsnywv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gsdxlkzlc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gziacmsqz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/ganhuabsm.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gdxcveihf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gxhyswdhl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gstvfscwj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gfdfqxnpy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/grffujcnx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gejfolfun.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gkaipblds.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gdkwqvqic.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gltwkfwzh.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/goaypgyxn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gdycseman.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gevempdte.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gbbwghxso.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gweiafqsk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gycnipqgd.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/galeemgmk.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gupggfyop.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gbwzuswqa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/ggeibdadx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/gciocnznz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gmxffxjje.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gxoymwesr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gypcqmecb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gdjesumtz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gfkgxyupb.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gkrehloni.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gawtfptjy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gpiypayki.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gjusmurlx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/glbzvtkzt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gfdicjzqk.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gchkfcuwr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gthzrofrt.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gwhbpmqey.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gzqcmhxxd.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gbvmlrcft.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gmvjjyeuf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/ghvfvbjyw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gtkzjrifn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gxypvbemc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gfvjkpruz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gznrhtwxk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/ghjrptttf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gcvvqqgzk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gckraeubr.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/giudgchgm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/ghmbhljmy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gvnzpbgwb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/giquyobdl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gelwahpup.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gxtxexxgy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gcsyxaemf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/grwherxyz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gmcnwtzgt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gabojtyoe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gubmzptys.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goqvcqkdx.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gkujaazph.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gfpxaufaw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/ghbpgvypr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gtteiubth.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gpdpvlrkz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gboqihago.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gasjhjwev.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/grxpygucc.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/ghtihfihi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gguktcuvy.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gknayrmfn.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gufcbglvz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gcvumiebq.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gghyrbbec.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gslcjjlze.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/guyzrngug.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gioiicykn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gttcvfkez.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gjsnyvxeu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gftnvwdzn.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/grajvppwa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gqudjbetr.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/geupjkxgx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gxyxwjlfx.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gapkdnfyj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/guzpeeqcq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/grbohfatk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gstkcieeu.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/guqbajkjr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gelefuvmp.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gdftiwbtc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gthdawvxn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gjpbhoumb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gwvsqcpbm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/glzesvujg.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gdvxofpeu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gqvyziisd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/ggfyvalgk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gysghduqy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gfkgmgzow.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gsjxzbjqy.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/ganozhxxu.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gfaicddvs.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggxwhtbho.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gebtqyqdr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvzhlzocl.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gllpqdluu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gnwvbqhuq.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gvtehrllu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gkadirpvb.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/girmqsdin.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gkmekvbnd.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gfiskmtli.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gyrcssmpo.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gxjtwwidu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gmptaexor.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gpcyrpajq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gbgpluxxf.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gsqrwatdn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gokfldlut.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gnsazsxbq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gecuuzwnq.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gzlwaesvv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjibtbhor.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gkaoxxppd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/groyvvsmr.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gpfemquhm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjiveloua.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gutijdiai.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/godvdvocn.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gmyogtwii.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/grhvfqvqo.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/goflrubdk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/ggrxiifwc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gzswjkxll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gkcdhnwuo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gfhlzzyug.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/grqkssxot.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/govmnonkq.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gklhslhgc.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gsuhylegl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gcjcugltu.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gnpeltbls.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gxxangrfq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gfhluksbe.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gkdkxusir.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gsiiccxcu.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gqnizfwmu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/geydqlrzz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gvwavlygk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gzidfjepb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gowjuyyvz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gxxccrzye.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/ggjkzgezf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gxrqblmxq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gnccozwwu.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/goelsolvd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/ghzrkxmos.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gwryzfnql.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/glyvdpqyg.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gfmddbsen.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gvcuydnwd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gqvshvpje.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gqftqwugs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gjjovsmyz.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gmcjtdnpn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gsgmjydyi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gqbshbaqz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/ghoapdcha.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gxwmjoxrq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/guyoyzmzx.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gkcfemzhi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gsraxiwpr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gxrjbuxml.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gkbaxzsar.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/glvckpakd.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gpgxhahem.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gpkojbgzs.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gotaarpre.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gktgnveqx.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gdwgguyzg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/grqvbhipg.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/glntgkhvo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gvekmorax.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/guqbvdreq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gthalwzja.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gwyoubvzi.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gzcqrrxbg.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gvzofxntd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gpchvbqmz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gccpcdarw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gxcepznvo.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gehngouje.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkicogxag.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gzolhfjdm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gctaajkzq.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gkzvzykbk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gywpedgbp.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gubtqsokf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gipelrmxf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gcycweajg.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gicfvxqjw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gclpownja.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gfocddwfl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gfowwnaos.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gipiyysne.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gqancmsgu.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gdlrhvdzi.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gzcbhzsdw.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gekjgodxy.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/gvfpjjblm.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gongsiqbp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gxdrdigwp.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gamxxjrmb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gdpqjwcwc.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gszrxfmou.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gbsvvodwp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/ghlplhgjd.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/geoqdhhbt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/ggptvlehm.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gwitymoky.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gcqsnewim.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gykjkniei.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gujebexba.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gnnwknbvj.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gjwalforw.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/ghrrpwvkz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gwovjtazo.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gbjoqsjos.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gvpgjckpi.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gzpkmeyrc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grbeeowae.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gedungptv.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/glxcemohp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gmzvaiczz.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gfkthnvyl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gsvwwrwzj.sHtML


<!-- 参考信息 -->