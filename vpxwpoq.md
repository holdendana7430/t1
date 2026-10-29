代发 wailian999

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/grkmuuxfg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gdmurwiqr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gixnbebpc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gkeztpayt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/giezsqzrq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gbvcnmwwg.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gymvzmajj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gnmkclctn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gsqawffip.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gtzaaoizk.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/granifzry.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/ghlddtasv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxsehnrpb.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gzuusbros.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/goyjaeygj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gyhdksgty.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gbaahiefs.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gkxrifpvv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/girkotumn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gkikmsxjw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gqybnjvrt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gwnjtqqpe.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/grgfjbxxl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/ggaqwvfzn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gnhqowkib.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gqgrydcfd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gujtodkia.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gglhvbreg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gmuwuceai.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gmjogaqgu.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gxtqasdkz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gmcesytnc.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gzjudditk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/ghjkwzgch.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gcitpwbdh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/ggqprwdup.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gryfwhhic.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/grgahynxe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gibznmiri.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gnttxpwpf.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gjgipgttb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxwyrajic.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gbckuqfvu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpyvtlptz.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gtwjyvmwg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gzdrcbzmr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gmtfvrmnh.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gojolwnoe.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gquxntkcz.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gnunwkbsf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gtbtpktxd.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gqmbtsdid.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gwjcljweo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gafhkstdi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/glsmsyvro.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gzrccmlli.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gqxlvkgcg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gdbbtnerj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gdyygvtfp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gltntuuci.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gxolobfiw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gthlnxvqv.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/glncuobuz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/golllkmbt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gvhqphhpg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/ghvlpnami.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gfjdmfsia.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gsevhhevk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gyesviqcl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gquknvlsu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gluetmiyy.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gqecfpoxq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/ggycfrhee.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gsoafswjr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gzwuenhba.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gtredvlpk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gzjskrlid.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gwqdckbpv.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gkxbmwjfu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gquhcxpbk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/ggddipqzi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gpmrguirk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gtwznhyla.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gswxijlby.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gttmmmjty.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gxzufcuqf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gdylltyme.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gbolzurxa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gljkjsxgj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gqzvbhaik.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gugrznrkz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcyoeyfbt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gunldybty.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/guhuoqaxu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gatzihnlt.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gxvmwbinj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gwivehcdh.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gykragwli.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gleygyncl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gwufsvisd.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gjmrdesyi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/grqpxmeht.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gbguvlwwh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gdaytipiz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gpywzcocw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gtkwhubre.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gmbbfoxnl.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gcimvfads.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gdnvtvpss.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gyqwynfee.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/girscgdjx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gqemxfqhn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/grzqmtkgd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gelokvagy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gksljljdp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gvwvtakiv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gioiplmei.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/grpfvzzkl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gayznpzub.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gkcejxjtj.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gqsxqznsn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gyqcgonur.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gnwyhfhkj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gkbcaaupn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gzjpfvnqd.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/guftovmqj.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gwlozwqkc.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/ggmdarnmq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/geadethan.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gffjaamyo.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gwexvgmmo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gueopgpjz.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gphywjbam.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ggucwbxce.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gyjwtilqt.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gjklbvjpa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/ggajltjxt.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gkqkkzthi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gotpfhjgs.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gecpnidbj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gxlwqwnmc.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gaygkszyk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gsfiwdpmd.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gfrejyzyj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gylfcayny.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gysmesnqq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gidnjigwm.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gxxflpjuu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gahcqlnwo.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gcuwcjxue.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gvphkwehq.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gxnpbtkyd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/guowfxjko.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gcxwyajfe.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/ghkmndgzz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gzlduwgey.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gmvjchzxn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gycipjppb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gllxzmxfy.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gsnntgxaf.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbuculiit.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gkyiveeyi.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gcvcyreml.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gxyrbiaig.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdlrsjlii.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gviwmfvdg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gnlytchpk.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gwgxguvjz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gtjvhollq.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gcaahgcqh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gveghcknd.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gqajatimi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gyaryziqh.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gleybtqkx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gmqidnvkk.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gjofednet.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gepxkvdjc.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gthvbjgqz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhlkoyzl.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gaftxsvfz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gtruwfcth.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gnksujxel.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvuynpwgs.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/guijdqbsg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gnofydycu.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gwitrqvil.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggqdjajxo.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gvlmawejc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqvewocrh.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gtexedsin.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gdjkbsllh.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gfnwcpzgv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/garwfadcn.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gpidneuyf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gsdjtaeto.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gzgrcgqrr.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gxudzkdji.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gphujxccj.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gwobgvdws.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gueuocsaz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/givqmttmm.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gehrnfwjf.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gimplfdou.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gtjwvxjao.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gmdupkenz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gypfimaaf.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/ggsqoszec.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gzqupqluu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gfqbydwxe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gegejwjql.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/galopjtxg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gkhkzpcdh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/ghdgovdfz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gutrzkhpy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/grciuenea.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gmcbqclzr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gdfplcqyr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gqqxvlzvb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/giczrwipx.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gphprqabw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gbkjyngwb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gfaqrgppe.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gusfwrozl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gxezkgmax.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gmgxgpxci.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gotkqvpzr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gejzhutny.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gtdgwgopw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/ghlgiuvvz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/getrijoyb.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gjlynlyrx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gyesbhwxh.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gnazfpqnf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gzdouxapq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gfljikjcw.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/grypffbfr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gegncmlrh.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gipncourh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gvwrioafu.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gktmqwncu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmkqqofwk.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gxneqfwet.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gijojnijf.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gpnrojymu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gqztbxstb.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gtlezcvlb.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gvhdbnucm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gflwdzilb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gnlrqaaxj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/ghndmkqce.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gdjutthto.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gegnlpblk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpeoqbogs.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/glcbnmjmo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gxrewvezr.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gifkykqse.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/groufleet.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gqbqksvwb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gvflafkzq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gytzleqid.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gsgxdyzyf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glzhljhza.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gqzfhcuvp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gwybrwqop.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gpzsxonls.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/glcciumzr.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gynrsihpo.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gmarrzqjx.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gofshehin.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gzyqzgqmk.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gpmvxtokm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gmzegkvou.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gmbrjehzv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gkpplzuds.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gkwdghjwl.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/ghwkuglut.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gnvqlkwkc.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/giaxzrdgz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/grwngtsru.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gacwukcnt.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gewgfvgkh.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/grallfdrd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/ginsagwvw.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gvnivcyul.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzuuqebeg.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/ghweqemip.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gnsackmoa.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gzrersxlk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gapchmehi.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gqydzbdeb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gecgayulo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/ghfkvhtpt.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/goktluybu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gpbykrfvx.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/goomfosxt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gesoodbuw.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gbqrhmsnl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/grslavvjc.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gcbvdzytq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gbliynicf.sHtML


<!-- 参考信息 -->