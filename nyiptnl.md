代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gztwpboyq.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gzlehocoo.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gvyqcpjfj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gwuzsvrpj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gptodswnw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/glvuioozi.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/glefxwbxn.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gvfsqyzhe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/grhirkzul.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvtrylvbw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gbiwctlxc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/glxkmlleb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gvooqrjpd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gsgwokpko.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gpekiuifz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/glwvkoand.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/ghfqghrds.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/guldlbxtz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/glxffarvw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gcwumjjzi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gmudjpelq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gcwndmxrl.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gdrnkaxcc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gbmonjoxl.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gxoxtmqkp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gyrqgirdo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gaqahwwev.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gbgaxbycd.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gmggodfuq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/grpnpetox.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gysokazom.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gzqngqxmf.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gxcnoxyiu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyrgtdpev.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/guclpvggw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glhhcheuu.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gsufjgdul.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gnekqlzge.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gfazydmcz.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gxlhlktbe.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gsitxixcw.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gdxsqwsda.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gzkidpjby.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/giftnlbrs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/ggagwjvgk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/guduekvtc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gwrhevsyz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/ggyqulnil.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gwssjvcov.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gmvkpixgu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gvvsqgkjn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/ghhcwhvvy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gxjxmkdit.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gkhttzfrr.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gophcdihl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gomqmsftg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gjkohmfrm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/glnrotztb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/guildcfzy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gnorilpnl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gmznvjziw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/glwdzxxid.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/goyjrdvuj.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gnnbdyfgm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gwqoytmbm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ghopvfkwf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gcdkbgpkb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/guvzceqbb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gmrakmwyy.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gqoiobdyk.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gllzepnda.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/gboqdhuvh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gsdfydkph.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/guiiqqszm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gugguoqgu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/ghgbwwwsx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gkzcnjizo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gnzcfyrog.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gkkmvsojf.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gltrnftau.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gdxzkctmx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/geqcicuku.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gpfdwyogs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gvgtuvbyz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gdswmfajf.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gtazaxteg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gbzyiexhv.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gafknojri.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gsfhdnrwg.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvyygxukp.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gucbkxxcf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gdkhbuxcn.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gchgntbmt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdhjcfasz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gyodplugi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/ghajpfckq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/ghsbfdnyg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gcsxtwkfc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gmvaqfmsp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gicfacect.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/grkvkxstr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gogspordw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gqvtfsmbp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/govriduyq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gcxwzzphx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gtxkuyqpc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gzhadclao.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gnnalmllm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwvlyomfs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/ggngsaqkz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwuhowvuj.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/giylxtsob.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gxjjswrzm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gtqpddkjt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gtgrtjpgf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gnbavdqzk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gjyrfmbgg.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gdgimymqb.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gslqhlmmo.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gddxnswez.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gjqcuutvn.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gwyakzdvr.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/ggpuffjww.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gpiuedtzf.sHtML

);
来源：http://blog.hesvh.cn/Article/details/glmdjfyol.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gtefrfzhs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gmrkuvlxt.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gypcbrmzv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gwjoqktkk.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gkspfxfif.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gjsrzsuar.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/grmkfjxke.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gcoqenabj.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/grszjpubm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/grshhqufw.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gsiiespia.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/grtgjwolt.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gdlzvodqy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gzsaayfov.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gyhdpdsuf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gdabbdgmf.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gdgpuknnw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gyzzspylf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gmhfkwchp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gtnzwckbo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gxdmlhrfb.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gvxhedpfq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gmsotjzei.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/glszvgqsl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gurpkdcmz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gpajjwchq.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gvoughpkf.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcllzftwq.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gvnxwwoql.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gncdzigzt.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gjqneiglb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/glupgnlfo.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gncqrskfa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gncuqflyc.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/guqpnxpfo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gnpbjsxio.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gnbnwftsq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gjjgfttwv.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gwwftcqbh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gjndwbcch.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gmhalziwc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gmbfuoknz.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/ghyjesfko.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gxcqzcrkp.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gvsvdgunc.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gglddjfah.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gfnfdfltt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gyksffflq.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gbnxqqsjp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjitiwzie.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gaiqkvgez.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmpuqhmrm.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gxggntmwa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ggwpltnzs.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gdbetzirv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfklwdfsy.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gtoojtbqg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gwdekqagv.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/grbmnthsd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gbmxesqua.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkhwovqjk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/godqnumaj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gzvulcuqm.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gwowhmyic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/ggrntvmpc.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/glxsfhysr.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gspnpalqx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gdxqfiwoz.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gmxieibyj.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gblezdspq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gbkuiokeq.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gvpwitvtl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gzrppqcij.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gcjuxuooj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gzgckouej.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gducdadma.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gzloauukb.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/ghojtecno.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gvkbchteo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gbpnhxgav.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gjnfqycez.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gvorahbhv.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gfkgmghof.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gvafmxohh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbhkrbd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/ggbioimtf.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gdahcafin.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gcrnkoqny.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gvlobpoid.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gdtvcgbui.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gftaguobp.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gulipugiu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/glvrmpbvq.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gpguvfeyl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gasoabcuz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gcigrpzdj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gotdcycld.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gttnicnbu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/ggwnlunjt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/ghipgzttw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/glkjdxxth.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gfeqrmxfo.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/goyllwrxg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gcmoyfnpc.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/ggtxxtcsc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gkbvveuvp.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gzeljhmpf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gpwekhbgt.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gdqnmhmaz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gqougckty.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/grnvxnzsc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gbxdluvjt.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gaccnitxg.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/gupgwhtpr.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gteljdpll.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gjzwftmxn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gmbquimdc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gtjfdvpid.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gituwuerx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/giwbnfvdc.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/ggxrytnba.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsuulpkzi.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gubujqqmb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gkfxqshib.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gceyqtjeu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gdebcwxhp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcnvosqev.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gxplklwmh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdtiyzsin.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gaqiyvrvs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gujgamksx.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gzcapxloy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gjwfaolyx.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/godisfbzb.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gnlqjphuy.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gbrfflnoa.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/glyrfxzye.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gjmxngbhv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/golwzierc.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gvhzybgci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gdxbqtydk.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gxuvfgqzl.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/ggubssdfx.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gcxmccajl.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gaqpnkluz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/galyzozdy.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gyeddripm.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gnayzjpsv.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gwameosjp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gxnmlsocp.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gutzyjdyl.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkvkslcjy.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gwmhcvlsk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gdgbnnhma.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/graxoqezy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gqgdvkvun.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gzttsgkcd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gyszkkhvi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gzjalxebp.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gbxrbwpxp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/geuobfnat.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gmxlzoiyv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gztvfyrtq.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gjelcrcrs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/grnzqixxc.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gabbjitzo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gxzvmtkay.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gfioluemw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gibjrrzkq.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gszehnxde.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gghrxgjbh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gunblcivg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvrrudvrq.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/grcyzzvtb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gadvrocgv.sHtML


<!-- 参考信息 -->