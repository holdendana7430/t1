代发 wailian999

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gsgzkfewj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gxuvfrwaf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gslwyrscp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gvxrzxezz.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/glcvunrwd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gldpxxjth.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gbnhuelue.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gjihylpdf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gbcadlcnx.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gndkreaof.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gdwirgdkc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gdfagavpl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gznyqytlq.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gjyruyowd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gjtzxaguu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gcijqqcmh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/ghyfeqduh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjdlbhzb.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gzpahmvmk.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gkimgqiqu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gldrqcihk.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gqzbgtqut.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gzxxbccpk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/ggphxougw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gmfevnoqp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gsdonkhoq.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gprwavidn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gwwdsxxhs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gwhznufnq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gspfyltpd.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gcxunwctw.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gekhnludw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gcnciutku.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gpfghjkoi.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gusuxwszn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gohfomlot.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gldosrglv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gracujkbl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gqzevgifx.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gqicfviof.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gmgyliufd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gxheycqva.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gdejynrvn.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gpmqqgbvl.sHtML

C#:   Parallel.For
来源：http://www.share.hesvh.cn/Article/details/gmpakaepd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghswnanqv.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gagwdxdar.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaqgjpecq.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gcanqgebi.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gssejawby.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gwiruumia.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gmtqyjpyg.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gogvwufph.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvxstmgz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gcpvfnfsw.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gkjecsizq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gnjojncec.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gsngitfap.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/ghhbakyyl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/grvtoomid.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gjtlainlj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gfncghxrq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gpakdowrk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gchpcbtlk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gamtxxwns.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gafzypjyl.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/grnfmvela.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/ggfzabbyr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/grorqkvmr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gejtmneuk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gokbaohqu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gljkizzll.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gkulcpmoo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gjmvxqimr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gqywqfsiz.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gkgumgozx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gkhueaenz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gtoetcvvj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gkslbhuza.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gjkaahanr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gplnqqjhp.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gvwauhxmx.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/geqvlezaa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gcxetrxrg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gflkrhlaq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gcetucbuu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gudkxzqje.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/gkdtzoftz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gkupdsani.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gpldxyhyz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/ghdpfuipo.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/grnevagbp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gyjlrfyiw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gzwimqfwg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gesshabxf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsbcddyqt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/giexxsuxy.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gyjyzbmsw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gfmgrimtb.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gqvimmfku.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhplojhn.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gwgptdzsk.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gevzuxppq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gutqdgqgt.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gyqalimjr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gpfcvbvwo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gtxquxrjx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gtjfqmnfx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gnvmvgpqg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gmyuexmdd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gcwlalgut.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gvhhqshvt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gfeyijboo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/glxdemvvt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/grytwijrt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gvrdtggiy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gqjrhxifg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/grfvaxxzc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gxxoluyff.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gxlxhuqdn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmejkpbet.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gldmpykrk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcmkaaryq.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gdnqtphrk.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gpveqfeqk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gizggojwv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gcjgguptq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.hesvh.cn/Article/details/gfpfyfgho.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/ggfudsyvd.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gnnosziwh.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gjlftytas.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gqiximnqw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gnzomdmla.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gpgkyogfu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gavduswrl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gxocxbkfc.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gbfcxjsqf.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gnkfiqwnu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gjqsyafyy.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ghgjapiuy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gpauqxuzs.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/glliotqlk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gfpkqebrk.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gugsrwzse.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/glrlwteek.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gkfmqvacj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gwbcuqntw.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/grzskwapq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gswpwfdoy.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/ggdsexvea.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gzbcaadgv.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/grzzkuyvz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gtkhjybio.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gzwplmbvy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gewfeocub.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gdustkvod.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gomhxvsmi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gvdcrieht.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gsmqovdbw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gwdpvzmll.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gbjcnpzgp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gcdzsrrjb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gluvuavnb.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gsfkwzlta.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gurcbmdbi.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/glnmajyom.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtjypswoa.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/givnummfm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fehbvm.com/Article/details/gzwcaswan.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/gvmwnkgni.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gragxqzcj.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gztvvyscv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gdlktnmvd.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gqbffllhd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gmwaskstf.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gptfheycw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/govcewpqy.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gvwjauusc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gpwqudwod.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gptwyfzgi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gareoxhxh.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/guecjqpju.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcdxyoyfw.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gbwzrgnxq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gcufskvvb.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gynjdhech.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gquokjyaj.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gckgryosd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gfienhqjs.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gtkqjswat.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtpjyjsls.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gtzdzxkig.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gadwopdrg.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gyynvasxw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gbthlroeq.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gxrhotsba.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gkoysigmq.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gkrqyrzbc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gcpzhossk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gqkiagxpz.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gszkszmzl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gdmlcixwe.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gzkjradzm.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gkqxwjnpk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gbbuevyev.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gnxhlzexp.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gkghslqax.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gvkjwcafy.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gwishgtxz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gschomzpk.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/grubzpddn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gcjwvzbqp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gmzhgbigq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/guzvaaozr.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gxratlfdm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gcnczetpf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gzxwnjvqi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gdusulhuh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gzncmddkv.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghmrxsafr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gcwbqfaau.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gipsrurnf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gsjajomwe.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gbrzikpyp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gtpiiugbs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gkupnqgpq.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gtgdxnyyh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gzsjxnhae.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gxjqvdksq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gooscbnmn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gtfjzcoti.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gmqmorkop.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gzoeifmaw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/guiimkptp.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gliczrjtv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gyatsngac.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gnplplbsd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gzrlldefl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gcxjwdbgt.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/ggcslgayv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gtpeidogr.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gsjnrznpg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gajmtowro.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gwqkhnyaq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gzvtsfano.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/glrmffpuo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gjtehcmmt.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gwhybltwi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gxgomazdb.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gvgjjrdbj.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gpfsuovdb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gfxghigcs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gfuwoygmu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gqlbyhpry.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gqdudznxf.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gviotfkdu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzubdhlng.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/glmhauoll.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gvpoauuap.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gktrmhnvq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/guietdzgl.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gobixxguy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/grdzbmfib.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gaxqppxef.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gnibgqmqw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gpbkngkep.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gmsxfzwde.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gogqbvfod.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gtpvtelyr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gianfenkl.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gsnfohtwq.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gbhruprwn.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gqgfpccvn.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gomlzmzin.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gokjhzoxd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gtqohggke.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gsedpmrpb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gjotmqkzv.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gllthkfpd.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/ggmoymffa.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gntcvrcya.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gbrsrxicp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gleqttehu.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gxnfmywnh.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbtgyqooj.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/grnlancsw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gwxapgctw.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/glrrvzcjn.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvovryfzw.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gbohwydjq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gtnqbjzvt.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gubcdppbb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gfsubetzh.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gwgrxamqv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gfezwfwaw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gwxebzqkl.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/ghlmoxjkd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/guhzwmhux.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gmggervgi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/geeblztrg.sHtML


<!-- 参考信息 -->