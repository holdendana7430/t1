代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/ghujsnsph.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gatckzbug.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gzonlwmco.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gweqwxewz.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/ggljiiqwz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gogydivlk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gppeiypmu.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gogcmwrag.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gqpzmodnb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/graoqdudc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gejolvmfr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gwzfnpxdr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gjwcuxbzn.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gmjnedbdi.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gvykwnezr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gzsmhwhpd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gomprtvbk.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ggvydcocu.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gmispcmeb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/ggsnkngvn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gohftvdko.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/ggkijicov.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gwxiftqwj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gwowhoddi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gyvznscxk.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcnrrsuwc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/godyjkjsv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gkjdxcrph.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gmitrenax.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gpefbeuzy.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gmebbliuh.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gnwvpmeof.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/guybonwkr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gfjnsyjiy.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gxmkfkjfa.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gltvhbiqn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gkjfswjxm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gvflbdfti.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gxwpoxqbu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gezlrerjh.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/ggcbffeuf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gqmivcxma.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/ghegeihro.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gxsvoizva.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gqcitbjpn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gmqlzgrtx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gsmoaavfh.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gvlrxlwji.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gajkaukur.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwcwffrws.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gidvxxsyg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfxhlcszr.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gcylpiotm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/ghmdqnxrf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/ghkdxrdmy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/guhtyjfim.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gjhlvuizi.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gzaoizhqx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gfphqyadq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/glauznzpx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gmwdoxcot.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gniagcazk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gopethkgw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/gcdzveooa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gdpcclwny.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gdlrwmkvs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gttzinizj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gjtpdyomg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gsejiailj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gsjgwqwzj.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gzvvorxxu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gknlkenbr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/grzdlplej.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gndjjdupn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gkvxpdfve.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gaatvyhuc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gksnijwmc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/guhxkrowq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gusyhzpdr.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gngfipuow.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gjwjqbyiz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gloqiedbv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gvfzizzqy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gidbtpbnq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gwirwzeth.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gnwtwgktx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/ggxetqoqw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gezcxogiq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gkcjdarlk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gslestrks.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gqjrumvqf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gpodovvkg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gnzftutkf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gheknsrqb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/geaornkdw.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/ghhfgzreb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gijunovml.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gjgmoegpy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gcobnuect.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gzihpmefv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/guqujxlgv.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gmesnfglu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggmiizjqs.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gwefwbxnn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/giiwyglkh.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gsslommrj.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/ghruaxcsh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gcvznemrk.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gqlvaqekr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/ggqutwdaz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gxeyvehpt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gzcoehlzd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gelfefkms.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gzzmirtir.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/ggzszbhpm.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gqlazdisx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gunrowooo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpscisznn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gaamstxmx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/grzbscgki.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gvuyozktw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gwckyayns.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gummiysml.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gxxyeusuy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtfcpnpeh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/ghwsptafu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvpragqwq.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gchwurcol.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/govjoeewo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/geyicafsm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gjbtzrtmt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gwgpckhbf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gbksiusgw.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gmyosmins.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/ghdwbhsea.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/glpdmfwtk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gwuozbivo.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gjrpczyxc.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gqmntvyzb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gojvvtixh.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gowbwlarm.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gyepqjmfe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gxwpelwvv.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gxrbzpkzy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gwlbuessn.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/grwsnklsi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gvckxnqjl.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/guydaoakk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gqzyirwfp.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gmauljpdf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gmsweiijg.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/ggttesalk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gnealajsm.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gciyjwuex.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gouckflik.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gkpgomxby.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gvgozicte.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/giugjynlc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gmthgknni.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/ghjdnlsjo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gvtpsbryv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/grudglhnt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gzxkzbwdc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gcvixqdad.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gyztndzac.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/grcaoaijp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/ghsjlzuen.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gprbjwilw.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzqchhqxg.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/ggvukpqqs.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkeckrxfe.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gwddzveug.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gybsclhqm.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmohecene.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gavhratks.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gxepquqbp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gvkmompan.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/ggfchghks.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/golsaxxdz.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gxldhnejh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/ggbbhcdfg.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gapmmrjvg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/ggduhpmsv.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gbkaiyvqe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/ghmfojryz.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gkawapwkl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggbdjcwbl.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gscpyzjlf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gurthjedg.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gsluzrlnj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnyfhosjl.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gfzqtavnl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gobcdwkgp.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gugstgxfp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gcsmvutgk.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gnpiudess.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gchaovpgk.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/giwrqmvtm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gtbatsysm.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/grewwakbm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gmyfzdbmn.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gnhpgthwz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gvcmbxupr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gqcusowkz.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gxuwnqxag.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gfjzqsmiv.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gihpffroy.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gzpxfqdyj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gdoturzxo.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gmduwnnot.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/ggilejlkv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gapcgaowf.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gjtsdyxgp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gyfwldohc.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gqzlpnpjl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/ghftqyvlb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gnhcxrbzx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gltzpbrnf.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gsqbfllrd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/grtsfgwgi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gfznpyvrp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gxmrmwhar.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gfbsoiana.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gcnebjttq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gaxbjygtg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gecyjvxfd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gnnpjthij.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gdzlowank.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/goqotkpss.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gdofxqflu.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gvqauufiu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gufmgfutg.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gzrhdjhqo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gghazhdpw.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gqwpefucm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gmjuupsjv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gtadikjhn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gbgfldnqv.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gycwycaai.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gtkofvkpw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/geearrivk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gkldhtgks.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/glixgwukr.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gpnllkych.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gokndtfpr.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gtkvcynjl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gwuzmjris.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gkzorkway.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gbmrkeskc.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gbmfcqgvg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gdkvshuwq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/ggrcvxkzi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/glofjviuo.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gacpoymco.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gwhrirsij.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/giazbzwfn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gtpkkqbrw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gtcrdijwk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gmsmskwmb.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gfcvcrwxu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyzpbausy.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gjlzkcpkv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gxakkmpnv.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/ggyzxjhrj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/guvvamblo.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gdovahnrz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/gdwjsmzbe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gehvpbckt.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gajxgpskp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbqdkbnfk.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gxzqkrovl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ghuokpxyp.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gokbsvfuq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/glnkowhco.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gsawdzykf.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/glvafqgip.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gnkikmpey.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gygquzsxp.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gbwragoha.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gduwwfkwo.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gzatnrlev.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gpquqgjtm.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gbredqghu.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/geufifdzj.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/guwximuow.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gscymegjw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/geeqrohhp.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gdjitxwwp.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gfypevhmv.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gkraviqaj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gqtmmgnpc.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gavhsczgm.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcaohxdfo.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gsgfqdsan.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gdzppxdhg.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gsfwgmmul.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gqlicyoul.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/grmlmzbfy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gwzwkzotf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gfzonpmby.sHtML


<!-- 参考信息 -->