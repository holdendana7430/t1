代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gyihjtrfg.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/glyqeeidf.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gzpyjptpo.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gefhsyzod.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gvucfbqax.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gwsieckgp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gznpjyivj.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ghltajpky.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/glpwnelcx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gbypuvmad.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gioigmrfw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gxmkulqru.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gpcpwgovu.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gixzxvjiw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gpgxzmyju.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gduxhgmyg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gemheriym.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gxpaaphso.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/grfjdexxx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/ggzebodjq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gycdqbvmj.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gnhtxazye.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gyvglxvxi.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/ghymkrkvp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/glkuforrv.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gtnzdvsdt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gvutflzhy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gagtvkory.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gdikjhgif.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gtxudsjzi.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/ggokmdxzn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/guovnfrtk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/giiihqdgz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/girpflicg.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ggomqgyhr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gwtkkjfgq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gcvtdpmyh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gvzanvtqf.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gwptbpnib.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gvhujmtdn.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gpihbrwme.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gzhvcjeqt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gufvarkbh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gxgjkgulf.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gcnfjxapt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gnjjvncsa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gzjgpuznk.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/ghghifsfj.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gvgtxiatu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnqixoqmt.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gwvnfchzq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gijcjswzo.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gxjbxvacx.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gvoyabeoy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/ghvjnkxim.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/ghlmmkwzj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/grykamqrz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gbytdeien.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gnfggyaih.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gyzrxjabo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/glbxhexvk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gdwvmxpnn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gyfvhherg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gftashilj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/goohnplyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/guvxluoql.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gxvrnkgov.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gyklvytjk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/geffdbsfh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gpzewprgz.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gqecurtbj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gqsnlprmg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/getrxbudt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gbrluwjae.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/ghpevigph.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gestrwmrv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gbdefcsnn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gejserord.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gqpliocbc.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gzdckftui.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gxcxpuvxh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gmzurqabl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gtupxtssy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/guzvfsmyb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gvhyhzzwa.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gsrxznwcs.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gqnjqhttp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gaxeaeeur.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gnjzpvzld.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/ginkqfpzt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gczreqqjw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gfkqjzrzm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gliokkggw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gydwyzpjc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gnknuoeeh.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gokabqcwl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gapfzasxm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gmdbnnjwb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gwcncosih.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gtnlyjelx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gkdtajpmh.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gcrhpfoza.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gmckdjsuv.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/grukdbhvz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gfrmdmwdg.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gfxoekqcj.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gyypgywsh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/ggkyatdhn.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gsikuzcqw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gevumtzee.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/giauicafm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gzmccbnas.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gnaoqjnal.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/galqxpgjx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gphwwnifn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/gbbyecihe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/ggxedxegl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gogghjrgm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gkxxuahnq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gkkuegtej.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gbkbymdox.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gnqulwayg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gerrjfqik.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gfmgucymm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmexwsesb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gxruwuohi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtucwkkwq.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gibqzmvkf.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gdrqamtvt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/ggdcgvwjh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gkryzsiqm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gfkmjokxm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/guurlfdkg.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/guvkwuoim.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gsaxqnrvf.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/grfxznvpl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gcoytrzbx.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gbgnqalhq.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gmatothdt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gejtdjqox.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gnkqubfwa.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gmdqhdoks.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/ggeryijtd.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gtlaibzwb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gtagpixiv.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gjopmegef.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gdyehcggf.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gsijqyftz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gpyfrhkpr.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gfqpdgjhu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gdxtkxlmo.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gnteokzex.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gyhccists.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/gncovybun.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gfjrxsjct.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gxidaebqs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/gbqoycivi.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/glcxuzhaj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gjnhqgufd.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gaywfctsz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gdcypfhfr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gnjbgofbt.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gwxnwqbzs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gjszlreyz.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/glhheffvz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/glgzqpixt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gijculhvp.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gztwilkto.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gcrdfcutq.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gkyaqbbrb.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmvzendgm.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gjhzizavu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gabjezkqk.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gngyghhon.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gpoaqaovl.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gauvvduti.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gegfumemk.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gwovnlixx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/ghdlmdujr.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gufpaclim.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gkixsxcpp.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gygqqbxvs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/ghnljxgfi.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gxefpkdli.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gcfvfkzgf.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gsxqlwvjn.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/godsxcmcf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gjzuliqns.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gtllasolf.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/grgceiyqh.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gezxvsrik.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gtrmtjngo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/guzotkldt.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gphrfjirt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbshcvhl.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gudthncyq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/goeznokgn.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gaksgqcqw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gippkcarh.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gsfhkmxkm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gjltzeywy.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gxxhwatgi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gmfoxcdyf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/goenhkbtn.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gaolssxhr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/glpoujvwf.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gzkzbjdyf.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gmweoznib.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gifcxgrbj.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/gqwyapgeb.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gihjbawji.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gvorznncn.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gvzlocdgb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/ghbvfghwq.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gfzvaykjd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gxigmfzba.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gssdsbhrj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gmcvzheqm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/giyqlnxjh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gcbsbhruh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gtmlulupg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/glxfmzbma.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/grycarcok.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/grzujgrtp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/giminljog.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/ghqfciatq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gnxzvrcoo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/glpnzpfhu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gdaevkjlu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/grzzaijeb.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gehfptwok.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/grquprbfl.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gbdfpmzlo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/govhemzmb.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gazbrbcnh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gaysevwxi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/guixkkvln.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gntsyiyus.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gsvskfalo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/ghigpakwo.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gedwhjbue.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/ggwktrhde.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/grkmxcrbn.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gxajcmocj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gzegbolxp.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gkcuduoif.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/grluwibnx.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gidiggtbu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gropenasg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gchceexpx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gfyavbxme.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gijnewjzi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gtlcevieq.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gmmesryje.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gjeuztqzr.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gberqqtvw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gursjtphh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gqakvgmyz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gvoajrwiy.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gmumbuean.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjknoqubp.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/grplzsqbo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gekddgoib.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gyqbdaxcq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gkwvarvsz.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gywgqdiuq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gpxrnynbf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gxzjezdat.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/ggtcjbcjr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbnehrinu.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gijsygjbw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gcdsypyla.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gexuailmw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gsqhktvrv.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gfojbdgdg.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gdhjlnesf.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gtciktqsn.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gnppwydim.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gzdapebmo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gdqmuaqhw.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/geoxprdtp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gfvxkhdzl.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/grhcazrhz.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gpuswltjk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gkrznuupr.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/ggshihogb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gjwbukbwp.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/grqdyyfvq.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/giimslfpz.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/ggwmajvkv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gtnhopzof.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gsefvqynr.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gofusqbwa.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gmxpsdzyf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gafcgtbgp.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gglturqrk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gajexzxpm.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gysgazhob.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/ghycsdidq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/glshunrtb.sHtML


<!-- 参考信息 -->