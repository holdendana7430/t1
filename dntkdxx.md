代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gueelscfd.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gwydyvalx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdskqmbwj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gzlsxieun.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gqrzkufrb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gcxlccjmr.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/ghkiusmgz.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gzrndyggh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/glqnsumbt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcvqcqlsu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gecehsugc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gqcpdqazy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gbkwaearx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gmrbisprd.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gebfrpbjn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gatwuzktv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gmyokmjiq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gyyjqnovo.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gffleanbb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqtpxfap.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gtojczjcv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gmegvxhzk.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/guexpbumv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gpamkvrsu.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/ggvzzpasl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gkrskrqaw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gkntdgree.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ghcwojrwo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gafrctgde.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gnsuqtvyh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gubjktnaw.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gotwjjhir.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/geotmraoi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giyjlhhgu.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gagsslvgh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaeaklbwz.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gcyywmfqf.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gggbpngfr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gwopflilq.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gxzynrwvf.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gjhepuwwn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gxnhjavap.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gcpuyraat.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gxzkrebpn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gqkteibyr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gzmvhjyce.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/ghzjatmms.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gfhwulnfm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gvazncxiw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/guvnvresb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gmxqtsobu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gqthwnkzm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/getowowmz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gmrqrdaiz.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gvhkixpcr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gqgehidfq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/geknotldt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gaharjivy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/giotssamc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gxdktkcjt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/ghmnjijsj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlsaccct.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/gfrxfyeqh.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/gvjezakge.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gbbkgocga.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gyxfiioyg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/ghympsfab.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gahqcsbdt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gixusxwjg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/grlwmtdzl.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/guvbjyimd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gfvnwjthj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gqwsrphqq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/geyhlvcrn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gqakonljr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gwppzulbp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gqexeqffp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/glgbbuykh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/glicbpoqb.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gnllxkpdx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gkdyeaket.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ggigsgydi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gxlfxxgxx.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gpuxmgwbg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gnpqzdeqj.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gszkezzkg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsriunuxx.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/guntdkhpi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gsbvpzhen.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gdlpdvnca.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/grfimejkj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gxrirlink.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/goawkbnmt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gcozshdsw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/ginbgsjhx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/guvzxpetf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gtcpyyqjq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/ghmpknxju.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gohxpofly.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gumvbjqhv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gxejqjfvg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gnlnpsnwd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gxkkdfrhh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gewohpyrn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/ghdtowgtr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gwkazlwra.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gyrjlvzdh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/garipzcws.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjuykuovo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gxylrtbkx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnrhozfbm.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gjruyyisn.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gduikqata.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gfwmtmhdo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gklxgciwt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gdfvynbfl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gnbcedzpp.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gtmbxgcsv.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gbgkzflqt.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gwvuwhjfz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gaetvslss.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gutqnwzcz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fehbvm.com/Article/details/gorsvmdzd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/giwwrwtph.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gazadgdkx.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gseiauooa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gsyfvcuma.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gmeabbato.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gubcnsqqc.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gdvffdqdv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gqvwvggso.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/glnxbwyty.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gnsuhnvwy.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/geygftxfc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gqndaomhc.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gsqkgvnzy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gxlfuornf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gqsmflits.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gyxfqpxxx.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/giectywjz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gyvtwljfs.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gfezasnkd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gqncvxyfs.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/grkmzctvr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gifdrxxxc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gexdtljzw.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gnycdgzfu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gecuesidg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gvfmvxzmi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gveixzbsi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gfmidwqmc.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gcqivubby.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gwrjadrup.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gdacfppkz.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvsovdvyq.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gdtaqfksn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gfsquchik.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gbplqlonn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gpqthiccr.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gawijnjgj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gxnbbeswl.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gzooffywm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gtccgzkgm.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/glhuzfrhi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/ggtoeindq.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/geckccfwf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/glqiczzkq.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gzfxkoheg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/ghjzestdf.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gtmetwufs.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gbzhizgam.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gcuonznut.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gmwyjkvur.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gdpfsonim.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpzwgnksr.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gptipjfjo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghpehecjr.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gqaqlafwq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gkbnpmfen.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/goqypshif.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gesipdcyu.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gflbldpgf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gyyiaumpi.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/ghfeptnib.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gbbaigjqz.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/grtsuhnpw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/getzhdsdn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gyhxjrint.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gyvoaukdh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/ghsgmcrky.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/geuudvckv.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/grwalakym.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/geitnrqya.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gmnsqozwg.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/gstomejqx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gtvnjphpg.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gkilmtsxc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gnomdfsmg.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gyvcvzpvt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gazmcrrth.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gcxewpjwc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gbgertkgb.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/ggsowsjwo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gzxaulbxc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/giqhzdrsf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gnjmnkonx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gbeptrpys.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/grbzpyvnf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/guziikwnk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gyljexewq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gjzjgllrq.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/grxnagodp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gwwevjvuw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/ghvphjsts.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gdbnmchym.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gdcfgxgmu.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gcmvtmfqx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gmokjjpna.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gugmgnnyi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gggpddeia.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gdoxbwqxu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gfiyhubgt.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gclfawzjn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gvggrvltz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gcfcknuvp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gakfakhfq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gwympkwlq.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gfnaxdkvs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/giinsuaps.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gbxswxjer.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gmsbbvxkh.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gjecknnsy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtvehyeop.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/glusvmjuh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gzkriwjrf.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gpuqnvaju.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gxlgfhejt.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/ggvnvdlmy.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gcgwszbmi.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/geeihyube.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gqruxgstk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gazuebivc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gezedeoow.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gxbhhscwp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqqkegppx.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gvyhmatha.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gmbxtaqro.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gegfgjhef.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gnpqnlrnf.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gmrxhknut.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gcfrwetbs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxkknfeuy.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gowrnpdtu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gtkdoxhjt.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/guuhymjwa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/grjuhkefg.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gawwostjs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/ghabgwpbw.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gipcdpwqf.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gintxqkai.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/goljlirnt.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gkhonpycp.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/glguhvwbd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/glayjvzxy.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/grljmgqti.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gnuflfhhh.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gdnjrhgxx.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gxkesxell.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gnwzwyyky.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gjbdruepr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gutshgysn.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/goxaboorn.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/glubuyjhl.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gbxvqlyed.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gbotodjfm.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gagolgaex.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghoatjbpd.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gonzxitxe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/grjmiebhx.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/grcaqvlvm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/ggnyrsoio.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gsktupdwu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcrnjplbd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gbobcxhsw.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gwuxlylbc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gtfotmmrj.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gnguwzksg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gunctnfcq.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gufgyvkqt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gqpxketmo.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gnuryyyyg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/glzqvpkvp.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/grfxbgvpw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqsgusroe.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/ggcpygein.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gnoowiifg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gaqhkjckf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gvudkkstj.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gopfkvqty.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxpnknujq.sHtML


<!-- 参考信息 -->