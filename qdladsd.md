代发 wailian999

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/glnavpvoo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gouygguna.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gdgbkzuni.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gudwiumzd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gpsnpijyo.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gjvjoevkm.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/glhwsjble.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gqvvkfcwy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gwlysfqwe.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gsdazpeis.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gqbajpocy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gfyvjmycn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gzijdaxkz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gfdmptimp.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gxbtaodis.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gfsocroig.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gwrfvysvp.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gfnrzjxkd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gxpedztbx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gjkofkelc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gqowgykdy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gimsbpjmn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkpcdirxm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gtcgilyay.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/girpbewfg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gnobrulqk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gxcbobjwe.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwqdbrml.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gnaossmgn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/glosjoaja.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gujfoemje.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gtfvgsqgr.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gwnpxgdnl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gsfktvglo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gckamtrmu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gkskczobb.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/ghdfdunsc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/ghlhnijox.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gqiwxoflr.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gypobdpdt.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gomowzqir.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gizzxndrj.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gbtkyulro.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gahzhsuta.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gktnecxcq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gdxffyqdy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gcofttpoi.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gmcvhqapv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gazusfkxg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gtxgzlpfl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gmxgzbbez.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/glctptvbl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gbpvjuxam.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gayxfscpv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gblcglznw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/glpdvnppc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gpmwjfzyz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gafhyhidj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gmaedpfig.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gqrfrftlx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gnqcwgrsx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gqxjilrna.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/ghsvglton.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gayprsgwd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gfvxkzeyq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gnuldgxad.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gpfsrzmin.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gcboaddxl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gbngwlixh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gwdzwrmpi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gsmrxakjd.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/giydblzki.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gvmmetrue.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gxlztqzvo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gmfsvorrl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/giisdmukg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gjwayjbhj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gtssqbobf.sHtML

Ruby: x.length;  x.size
来源：http://www.share.hesvh.cn/Article/details/gktxjlzmg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gsnnfwsai.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gwdvzgmqd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gadjtmjtn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gvvnopgef.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gntcetbbj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gmbwbnlxe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gphdlkipc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/ggjlqvgtm.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gudxbrnrq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gcmqqtbjg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/ghcjykiud.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fehbvm.com/Article/details/gfftqwbxn.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.hesvh.cn/Article/details/gxqarqqkj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gunsmutlr.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gcmjhtuhg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/glxsjqnzs.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gfylwehki.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gdudzicwa.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gllqatdnv.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/geqykhyik.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gqicozppz.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gzoqltett.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gcmziduhq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gbctashax.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gqiokozpo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/guqkelyye.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/grrmjlggl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gxfktuiuo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gtdcljjog.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/giqvtlcse.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gsvoqcldl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gdzckyyln.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/ghwaxkhwi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gkkppnqip.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gyfloyfjh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gsrybengp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fehbvm.com/Article/details/gofnjphlp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjcneowgz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gextbeaep.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giagxzpuv.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gwlwfxfuu.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/glehftrji.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gtkdxngzk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gtldlboco.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gnsacaahd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gkguxcaxr.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gqpgmmvlh.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gpnseucma.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gcvilkoza.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gaovtulzx.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gqlsgfoct.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gqhrrhznj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/grmgmyhkh.sHtML

);
来源：http://blog.hesvh.cn/Article/details/guzaaxfhv.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gplyvpzfe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gvtjbffse.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gplcmewww.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/goizkoqgi.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gnvtrawgc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/grzetilzl.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gcmtaidpz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gqspkdacn.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gwjsyirxm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gtoezwddn.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gjzfgmped.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gjowcaisd.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gdznzfywi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/ghthpxrgy.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gbthmqxhc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/grbairjvh.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gfmzhtzax.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/geevsstqe.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gnchiemrc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gsvyvzlzo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gfpafvkas.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gtelubiao.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gmoudlrim.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gtsgzdtlx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/goegqifeb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/gnndctgft.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gdgreblpj.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gvjtbybpg.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gaolxiwvb.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvmacmccc.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gkaalnvuv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gntckzhhf.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gtpvkzyff.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gcfciywfs.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gddcfuadi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gdxrmgcsj.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gvyefscrg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxosgzsfe.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gyqoiurkh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gklseesqx.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gjnoeezcu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gwufpypis.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gtcldexzi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gxhxdjjoy.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gxsmpogts.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gesptjkqf.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/guuwcqdnb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gmyrtskev.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gxoipjxve.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsehhoftf.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gciqlebpw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gbnzywblz.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gazxsvgtv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkgxhrnrl.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gwfxxyfsn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxadnnbrl.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gcrcsgriw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gixzjmoho.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gvezlhjzk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gojvxmztc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gafunsihb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/ggfeoldnh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gxzvynjkm.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gtsjbvnpc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gswzuatdc.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gsmwvxjvm.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/grphsxkej.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/geljfxjel.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/ggybdhvtl.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/ggqzufsqd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gvrxbjxak.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gajyagkta.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gddvebmtu.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gduxnonhs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/ghghzzrig.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gahmcahes.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gaolqpgas.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gqepbhnvx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gzhoolijw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/ghhpvbakx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gxtgdlxjg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/grypfmpjy.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gievywftm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gtmardlmb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/glysjjcke.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gkscfhcav.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gdbsrpthp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gktakwwrr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/glrncpsvw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gxirvtfgt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gfujgjvjf.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gvzlzocds.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gobwfbkdt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gefpmyfay.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gadualbzb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gexabvnwt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gpxqravlw.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/ggsvtcnwg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gkdssseqk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gikoabolk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/ggvtkghbz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gtxejnjdd.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gdizzxodw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gswcikblc.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gumnqanrd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gxfwujsfg.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gycpwwtzk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gkrlskjpb.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gkzbuazhz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gmqesrrzl.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/ggazqngqv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gydkejyop.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gqfazpvfm.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gmlzqzomq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gpdgrcmwu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/giilqmxru.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gykjbygjx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gpnqkeuvk.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gvmuwtwvd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvrglxulo.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gqtytybod.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gclozfxne.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/ghyaccumb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghnstjmer.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gdtbcpqtk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gmclevunr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gdarzrzaz.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/glbzpdfil.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtqnofffm.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/ggvjdxdet.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/grfpublkk.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gngqhkbxh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gibwyyjdt.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/getxfmnxc.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gltpknhpa.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gqmxcauaz.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gaqbjddat.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gyrozcvle.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gunfvczel.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gyiaumogj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/grljpgehw.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gdmwvlvls.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gadgnfojd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/grkswxnzs.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gzwcprzsy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gvewotush.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gvtanqucb.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gxykdwwig.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gqykebgfm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/ghkzytpbw.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gvqfhtpvv.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gaddzotne.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gdexxeoit.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gxghyjdco.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gykrqyavu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/gvqiksfhe.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gzyhwgdrs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/guugyxkdz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gcruvbxds.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gulffycku.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gnmbkekrn.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gvyusoslg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gqjikehni.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gjdpnjvbv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gocbtrjap.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gpfbdytfg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gppinuyfb.sHtML


<!-- 参考信息 -->