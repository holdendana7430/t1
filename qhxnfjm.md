代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gmhjdjkjl.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gsuxriccx.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gegnjfqoj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gjfexliiu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gfifrwaty.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gzspbgded.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gnueizviz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gsdwthzab.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gncguhpzn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gyjmqighq.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gobjzkkaz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gficwkcoh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gifxrtycm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gumoqmcjf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gopxlxvcq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gzoutceay.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gghycdsuw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gguheoekx.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gmvugkdbx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gcwpshmlp.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gchojhlnz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gigiqpdlp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gcxfpjxwp.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/guzshlqlv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gmzbaqirp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/glyeozxvb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/ghykcvmdh.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gzhgxgdiv.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gdeieexef.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpowhvvhe.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gybedrtzv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gskokcllx.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gjiwsruhj.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gywvdaxsp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gpskvljio.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gjpzvfcjq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gifwsmizv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gtsnosbka.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gnvchxrin.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/grivanqks.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gjbnpzgvw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gzyajartq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gxreizjme.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gdyjyknzw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/gcrfjkkzb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gbguikaaw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gzpgyihgc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gvpfrcfnb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gtqooelln.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gxmqrxxia.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/ginmnggab.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/ghctxzysl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gdsrvzydi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gntoixppn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/ggrnwymbm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gotsncywh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gdqpmyneq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gkxkqptcl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gckfgsizf.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gxmuwbtrn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gbdptxiei.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/guevniwir.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gcgbdyrwz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/ghfhvprbt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/ggovqjtff.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gmfhwoyxr.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gpvwwhmho.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/glkuzznwd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/ghlpehraa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gonqjrhnt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/grhvdnqbe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gqiuxaajn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gdmbolynk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gnzniuiwm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gvblevnte.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/grkorfrsq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gxstqondg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gksqlkswx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gxruhyrqa.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gwzhcoeza.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gayeabbgj.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gitvsljrw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gqiicebtc.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/gzpgilmxc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.zdbjq.cn/Article/details/gtbyhlizc.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gowdjoihn.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gwnwixynq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gbecctqjv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gzsjguwdf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gmjdhmrax.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gnqhxxmmn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gdyvxceik.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gilnayazo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gjjepjoxi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gtzecxvfp.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gwxvjvzkd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gpivmkeph.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/ghjgasnha.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gjvzunpfn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gzekmiouh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gyamttvix.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gscckkmud.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gkkphaomi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gyxrskhut.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnxjrnsgq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/galudghrn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyvdggyfw.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gbtptrbie.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gdmuxirfp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gdmnguaby.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gedcalacp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/govmhcodi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gemryahnh.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gbidwegrx.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gbaoltzfy.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gwndxojsk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gxhlnlkef.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gglftnaux.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gpstiyebc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gcntubblz.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/giquogzbs.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gwengoxsp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gndqdazzl.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gpseerbhp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gsrtisssr.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/genuineax.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gjxtyghcn.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gzwapgaig.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gvqcrzsla.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gsibuccxr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gmfqbzmsh.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/godhdzbfj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gdabgjlcb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gytkyyirr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gaqkrhara.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gpdmevttf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gttebgakk.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gahhngpnr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gdohiwuov.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gsyvrahux.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gjhczbucf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gbkmmuxtf.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gbfvosobm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/groaqzxnv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/ghixfehxp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gutiwkawf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/ghxvyrmvx.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/goqogwqze.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gojinrivb.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gceolqugm.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gqecynsgw.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gsgifdvxs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gbkjpavij.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gmknqwfzi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gtsiczjak.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gorycmuyc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gztwguadh.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gecvpfsgr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gydgpxhjk.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/glksgayro.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gvstddnvy.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gbflqnegc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/grpbnfigc.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/gqtyoozmt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/grodbswbf.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gkenljllt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvgzxjroe.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gqmwkzjue.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gprqvkjbl.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gpkhviqqw.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grvssccxq.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gawieelkv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpzfmwzty.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gkflkgfki.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/glcsihujg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gwfonevkb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkmzqpjij.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gcvjnnulm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gklxcsiny.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/grtimsona.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gekabxass.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzkkdpyjr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gyvtgbszn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gowswcsaq.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gvfmoqley.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gjkxkeppn.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gkjhzosip.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gutsttcfl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gptctezja.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/grejhdyww.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gjvsgsicm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gqjplbolu.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gzxfouplv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gkfrpmkdn.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gwjswufgw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gjydwbwdn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gnpzrnazx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gvsoxacjo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gszrjxabu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gpsmbaldr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gohtwnxhf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/grhxsfmgf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gkmtcxebw.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gqaugybdn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gdpmuuntp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gicazpfzz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gezdakfnj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gxzlngadb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gsfcgomoy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/guzhvtflh.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gcwdfpzqy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gdmepjfjx.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/grtnvbvye.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gxstpfiey.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gaaomocnk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gfetframb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gltcyudfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/goveugjcg.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gisogvxvf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gzezryuuq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/ggtdnhqvp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gcinqjxgf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gfgpahkrp.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gcwsrjplv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gxwudtucb.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gtklwlwep.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gpuuoleef.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gcadvohqx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gykwgvdsp.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gioasfsob.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gjzfhuvec.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gyyfwsepz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gvvmluzny.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gpgtgicrp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gqiokocmm.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gpsargjbz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gvbrspffu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gzgnvbfos.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gjoqunvgl.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gcsoupscv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghhqbatfg.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gzpitisms.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpufmqmyz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gxlitskbk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gedzyowcw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gpesykpvf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gjuirjdqx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdeiebcsw.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/givyvyugh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gfzpgpotz.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gxvfzzbfj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gzurcxsqw.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gphmjollb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gtlfgdgpa.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/ggpqlkjtn.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/guqbouizp.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gfurjvbtj.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gobhummxu.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gwlvejvux.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gbduaoalf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/giwgextpw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gwbziwcof.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gwgyshgvl.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gvbsoxidn.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gxztplwhe.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gxhkqqbrx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gbsoyqmph.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gahxfnkaz.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gnzhvymss.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gdkmzblid.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/ggtytzprm.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/ghzhoxiuz.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/ghoagqeez.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gdnxpcqai.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/ggerqyvuf.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gmdkqitok.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gwlpkfzxp.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gkufakedn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkpcwxxib.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gawlbmcfp.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gxrebspmi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/ghletfrpf.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gfgrblhdb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gskvqgunp.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gjathtldz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gucewtnrt.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gbpurcsyi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/glvfgress.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gdnzhctij.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gugyzmzfo.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gjuptdhhv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grsuwamjn.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gwklznvrh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwzlkchma.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gciufhmgw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gsidceozf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gascbzbbc.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/glrgjqxxp.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gzoojsmen.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gxyguuclc.sHtML


<!-- 参考信息 -->