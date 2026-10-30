代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/glgehocgd.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gpbjcpxak.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gptvezcsm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gjlgrkgbo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gtuenpnzu.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ghltufmzh.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gbjkxvpnd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gpdxjfukp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gvrrwruoa.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/grpkjibje.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gmwdawzme.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/ghvsuugaf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gnqwbjxsa.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpjcgpvug.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gsciaixih.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gktuuvqxv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gugsepvky.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/ggjcoljar.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxoqdvuge.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gqzecctzr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gjepkoejo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gvexcgyej.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gvumqwuhj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gehsyvbik.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gjsabvqhh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gbbnhyqvn.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gbqzpszar.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gmzqjjwad.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/golyuzmjh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gmequsyes.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gmclkojiw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gkntqszfz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gilupbjic.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gxnobinwh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gptyrgqqy.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gzqpigvdz.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/giaovaevg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjcoywzaz.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/ghumitzkq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmwsocxyr.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gkodnkuhk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gqrmgqtvc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gaexkholt.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gsgqnwfqu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gerawyqya.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gyrkdfbnr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/geewtsalp.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/ghfkdqqxi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gslccawsi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gkacqpodj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gbuzvxzij.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/globinoxc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/glaupppyb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gsgvgcwwo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gtosjthyu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gpdxydrkh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gsieqtghq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gejyddoyn.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gsvkecafk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gpxwomxvw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gsozlwwxb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gjaoonmfl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbuhnwvvp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gcgbmferx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gqvrvgljb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gelthrqfr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gideuemus.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gmczpamdf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gacernetg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gplxeshrx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/goquyytzx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gpdjududr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gptokiuyf.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gqsswzyke.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gtzyfiyqf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fehbvm.com/Article/details/gmoosxfwl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gwcrbztyb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gahahbdps.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gpgbjxuff.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/giiurhyuy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gcbobcavf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gkooyerfq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gvxxzkbbf.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gkygpjbiu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gedyhcknf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/geoebvrgu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gkxktzefg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/glciyloab.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/ggskqbinj.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/glbaiqjdb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyecbrvvq.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gftxlclpx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gcwlrfzsl.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gcpopeynu.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gxtswfeav.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/glhohtlpn.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/ggkuzioqw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gbeopbgjz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gmbbpjoxt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyvockhuy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gnnefjxvr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gavagnbbt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gipwvblwf.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gdyznwhfk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gpfdnadad.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gzfxrxeef.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gavxmimcz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/ghrkdiqld.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gimcihlra.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/govacoxel.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gbjsgjqfo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/geemzgenh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzcqrwkhx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gvixbqlgy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnewryboq.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gunccniae.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gngnqldkz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gheiickmg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gbrudlxgd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/glzbejtwv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gcjkrjrta.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gutejzili.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gpyzbptjy.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/guuzpwest.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gidsmwyyt.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gjhlgnsqr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gmrwwxrhi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gcbiogqdy.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gkhvsutqu.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gvteoddue.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gaaqixvct.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/glqtuvhot.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gjjerusvd.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gcxqpxtmu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gtgsjqfce.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/giwjtikis.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gzttnqitq.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gtipynkmd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gwzbfixuk.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/goierunbe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gatkmebuq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gxvcdpnmu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gftqkzrff.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gjatvstbt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwpfczdth.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/ginjsbsnu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gmgwtsbjw.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gomzqlvmx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/guikvnorr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gdhqqxewz.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gtdpslbox.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gepzdhmni.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gkmgumbyr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gwyqbomvm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gcaauvgia.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gmnxdkxkn.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjrtwwffy.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gjgavqxbo.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/gkdylzybb.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gxkbtckym.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gymuvoixn.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gqmwpyhtu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gynjbhgxh.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gjeqzawbn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gskigbaxp.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gdsxmdiuh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gfiqqtcdn.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/ghgjyrkrt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/ghkqbhykw.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/glkbwaihb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gibjbaday.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gkuqatfrg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gegurnbml.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/ghuyjsmpm.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkrvavmwl.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gxxhncuaz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gvybxjyao.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gjszezsbg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmxsdvaax.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gypmyrwtr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gragnlaws.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/grmqkspbj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gkamnrvdh.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gyxoctpxi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwaexevyh.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gjpjygzmj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gecuwrwgc.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gaecffiuo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmgwkcbh.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gmogthzem.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ghbkdbvzs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/giwlriqxk.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gydlohdli.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/ggkyfsgtd.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/glrayjloa.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/grfnvptjm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gpwldvybn.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/geecubhkz.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gpgwavhxd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/guljtvxdb.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gqhtgnpjf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gwzezrelq.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gwwdniymq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gmkoepqzu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gxmxzpwhq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/ghhugccut.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gasnavzax.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gedtoojlh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gsecgjbtk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gvsmhjjml.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gxncmntez.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gsfzfmwpz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gewwhxgkc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gcvorlcla.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gbgoibmhi.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gnqruvcxk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gbbanwtlg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/grtcnuzfd.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gboaltolu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gnalrbheq.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gzpfmapvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gcyjgjhwx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gzfgcgall.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/giojpnsyp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gggdncsck.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gemqpssln.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/ghdvutwvt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/ggnrdyrgo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/golxnsfzc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gfzpeplam.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/guyyzdfpy.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gbbnleimd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gpohnauhs.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gkhnyilhn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gbuaylowz.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gcwccgqhe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gelgbnccj.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gkqtlmjhq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gzoegcrlk.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gebyfbhay.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gybudyulu.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gfnkwpalz.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/guznxdjju.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gyahbzhrk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gpprsxyxa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gseloixeq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gfswnqamd.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/ghmthnmih.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gdoppvrxw.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gfmsvzzbw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gvdlsgunx.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gcxfuidkp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gcnczkcvc.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gpftjeklh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gbmyafruh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gggmnpihf.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/glyxjzrer.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/goluucadw.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/giyxfkucm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/glopoenha.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gggrhefqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/golptylho.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gozgfnvde.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gtzbuppax.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gvuaixnsa.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gguzefiib.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/gzxajsrvn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gahmrsqbg.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gquqfhzyx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gdnznpvyw.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gvkfxzkfb.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/ggyynngvr.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gqsbahjyy.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gxrvgdzjl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gipibupfw.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gtfdcfype.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gpbyyirdh.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/ghnalcllf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/ghmbmoitc.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gwsrtjqqc.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gfzcouumy.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gwfddryxj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/grraojqzm.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gwrzprexu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/graylskro.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gdnkfcnxv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxbeygmzx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/glumspxja.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/guqlvjbad.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gzfnujtpj.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gysrmrpyq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/grofslyhp.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gfupfcusl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gjmiljglk.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/guwjnsedb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gworunysg.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gfqxjhdts.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gauoqolfn.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gilhpfrwj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gggdyzwld.sHtML


<!-- 参考信息 -->