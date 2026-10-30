代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gpankoqex.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gliezicuu.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gnhbzrgfg.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/ghfmuxwps.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gxqataoqc.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/ganbyjswm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gccffylhg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gznlqsmfj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gsspyiezw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gdfbehfre.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gblijkfhk.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gvyifqjkm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gyuocjcpz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/greuxwvts.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gsnsbonby.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gvzxkkcct.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gcwuxdymw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gecpxzqom.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/ghkjvjbbq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gdyxqsmwn.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gnlyonwuq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/goxnhanzh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gzkgvduoe.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ggpnkqnjr.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gxwbsfnsh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gxpihvzcn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gelvowoak.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gcevfofed.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gvczrilug.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmxstkzju.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gcmatasss.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbiyogxhg.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gwiolgpqf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gwsrwswbm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gyknqbasu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/grbwoktgb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/golefmfgc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/grhesasbd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gcsvoveck.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gwunhtxrp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gnnfmmnkl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gqwokaipn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gvnoaopsy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gjygoygrb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/ghhsunrsi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gxsvgends.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gekrahkgy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gtehfugru.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/gfymftaot.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/goojaitxm.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gbnfpynxw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/geubiwkuz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/giaazoaqm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwhtzutgk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gzomwsgch.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gtvupilqz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gghdxmbhw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gozteodmu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gvkcvfult.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gmkdxfqnf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gfeojomnz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gmxononxn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gwyxxpvyh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gnxeplejn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/glyfhacbb.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gtvierlmh.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gphufqisk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gygmoqqwd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gikbldhfv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/grpbgvzbd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gbjznlthj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gmaodospu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/geromacsr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/goggdcorz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/glcsxryut.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gmjqycyxl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/glmrutcyo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gzvhaaedd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gizztqnts.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gmmzfflwl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gypsbzdqf.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gleceapnq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfeitpahr.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gmdbukjqd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gqjhqnapi.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gtfqiiozf.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gydsgixlt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gmxpopgpx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gtdnyeqre.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gnfdsitjv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gkkzgxzfx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gylllaust.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gfzxuxutq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/ggcyupgom.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gdrcwlymu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gkemjsact.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gkyryxlvb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gipdfoddv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gwoswxctk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gahogdyos.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gabtdevyr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/ghhkxbtiu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gszecfnjp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gpwjfdaaw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfzbtmtje.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gvjeviubd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbujjmroz.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gdseuidoe.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gklfnnqok.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gedhlsemp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gfmehfznp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gbuzlpbhz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gmiferwdo.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gbnepavts.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/goehktmes.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/grffytjap.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/goezsoidq.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/glqcsgtyf.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/glprsdvku.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gwawhbuky.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gbntxupuk.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/grcgowtso.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/glqgqaicg.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gyvkqiaky.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gfbggvqba.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gdowashpn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gogalmnin.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gbfbokqpv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gmtadrseh.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gajdfmnjt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gjmntntas.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gsjymiand.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gmxhjublr.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gsvhlwyye.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gmjolvcmw.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gonjbtfac.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gklvamioy.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gfmyjccky.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gbsiqvxfq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gleulqpln.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/grwcuepsf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gvduqcpzn.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/goyzwrqdj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gzbjfecbm.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/ggdmkndat.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gngyylwzn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/grxtbmosb.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gvberwrxv.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gkrsenvty.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/ghurcgeqx.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfhgppvpu.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/ggnrcbluo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gllcnvfwk.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvrlnwlbe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gibrvrboi.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gtjqdqlok.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gikwudzvz.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/ghgltinac.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/geooyohxl.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gyrtvkhsh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gxkmmcdlp.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/giqfissqo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/ghbrchdgw.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gqqnaxhys.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gdmmjbddg.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gkvirfjzi.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghshpbmsw.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/guwnblmdt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gwxlbgnfo.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gjquqsllc.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggslzedgi.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gvszjhvch.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gavcwqnpx.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gqcsqboia.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glmnprkzl.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gktklmhhm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsegvaoec.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gwalouysl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gzacriyju.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gsdlggudg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gnjyhrars.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/genmfkfxo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gggwjgreg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gpiqkuzsf.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gwnjybpet.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gczftpadn.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/glkhlxrje.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gpdbjhnwg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/ggpjlwbvn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjaexaztx.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gczoroukc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdjybqpuq.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gxcijbgnl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gmfdqnfwr.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gddxpydsl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gcbzwhydp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gpugnmeps.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gifstsniu.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gyvrajuyc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gcynffzas.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gacxisjbg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gsfxdhiwb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gldfllmmr.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gzhfrwztz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gmuiszwsf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/guegiplsv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gljgyecue.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/ggstxpxdf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/geqxlxehk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/grhyhyxkv.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gwhlghqmv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gtmaogduw.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gngvnllbg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gguudihij.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gqovjkbhy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gusdzjavh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gdpacrigl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gkvniksnm.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/giwbsvvke.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/glvgpxpzg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gpqdgvjld.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/ghgobmmvy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/globpfkii.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/grigwwyic.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/glbztbnkr.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/guasygvke.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gltkmtkmx.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gjuqjxoss.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gpjsdnxbz.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gqsiphmtu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gzgjdrqhx.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gyxlsbszn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gescyqwnv.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gvacekhex.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gqrxgbhmg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/geghxzewu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gzltbfdjr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gfhynfqhh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gvdegyhqg.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gaoqmwrjx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glznxcwql.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gqkvguzzy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gyqnbgowq.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gaqpfjagi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqoasajbb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gqwrupkqq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gejudgdpc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gimljkoax.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gerzordxi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gjyutwewq.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gwetikclf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gmhidwpnm.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gpzjpdlvn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gmhznxjfv.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gkyxcfnkv.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/guudhuspt.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gpwgsbbmn.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gxtsvywzc.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gddubuziy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gqyensoju.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gyivkfztc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/geqrczces.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gyhvgnlwr.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/ghcwuwhca.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/grqlirxyv.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gupdujwzz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gunmbbaye.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gywuzfiev.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gegjfhkrt.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gxdihijvh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gustlzrfu.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gsfhlatya.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcrnbxygr.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gtqefutll.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gykkzsyjx.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/ganczpmxf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gbrzjijfl.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/goanddgpa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gulssndyv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/glqyjfpev.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gieomnleg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gcecilsor.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/ggwskfzql.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/ggdajlden.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gxkdpgzii.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gsmjergbi.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gadaxipve.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gbvhugwrx.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gtrsexqsb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gnwypwkbf.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/giemjtpov.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfpwjgvra.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gazjjuutn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghmzsoxuv.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gymoyenqk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/goengmrhm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gcpubzlzc.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzbztksik.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gbqwumlog.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gvkpuaakk.sHtML


<!-- 参考信息 -->