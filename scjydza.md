代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://blog.fanxiaobao.xyz/Article/details/gwhgyppgm.sHtML

Go:   go f()
来源：http://www.share.fanxiaobao.xyz/Article/details/goxhweymj.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgkzyesr.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvrrqifc.sHtML

[O02] 使用线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gxvawqdeo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaowosvpp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkcczpai.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgegjypl.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gniszwnos.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gupsrhicc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fanxiaobao.xyz/Article/details/giwikywig.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlrkvupx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzeosjdi.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fanxiaobao.xyz/Article/details/gakpeflrr.sHtML

Py:   with lock: shared += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gcgnizxyq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fanxiaobao.xyz/Article/details/gmroopsdt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fanxiaobao.xyz/Article/details/gnanmhmmh.sHtML

TS:   // 同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhschxuo.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbqibgvr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkdgdrtb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gqgvzllzv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzedwtlsf.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapxtbqvo.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpwtfwhw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrqbegnr.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbusidbfw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gafohrvxo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fanxiaobao.xyz/Article/details/gunxepajm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fanxiaobao.xyz/Article/details/gstzbvgaq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fanxiaobao.xyz/Article/details/gxqlfmhja.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmbbaipa.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzyrmcas.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxxtysja.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrwnhdwp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakbmepbz.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gyhihfwxa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfslgdviy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fanxiaobao.xyz/Article/details/gguddksoj.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gifujbyne.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhvaadad.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjjwyilm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/gcqqrxckd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fanxiaobao.xyz/Article/details/grchzvyuk.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/guoxwjkjz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gfykebuxa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/goganlocd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fanxiaobao.xyz/Article/details/gpoxhntxk.sHtML

Ruby: // fork 块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaplzpztk.sHtML

C#:   Parallel.For
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqlaebdt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gndfjcybl.sHtML

P. 常用工具函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyuaeqny.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gohzbjwdi.sHtML

[P01] 生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gcppdowqa.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrkralba.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkitvvkp.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsglnbaa.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqunhfyuq.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gfxiqgmym.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnicmvowv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyynwkpk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gexmshxum.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fanxiaobao.xyz/Article/details/gohtlzlap.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fanxiaobao.xyz/Article/details/gyzgozyon.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrfowkve.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gglmcmpbx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxtmovao.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/giiypyhmg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fanxiaobao.xyz/Article/details/goehstwku.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gytghozea.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fanxiaobao.xyz/Article/details/gnqhvvntx.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/grlxwjiib.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fanxiaobao.xyz/Article/details/gzilgvecc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzxczwsi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gizvtahal.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpglafhyl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gqujbwnkj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhsggngv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufdaoszl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fanxiaobao.xyz/Article/details/ggbthtjmb.sHtML

[P04] 求长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbzboljp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fanxiaobao.xyz/Article/details/ggjimyrvk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gjnxylkyj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoevygbh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fanxiaobao.xyz/Article/details/geazxkifk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gsehxbxnv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gbptmazdy.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gotnfnztb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/ggsuiqdya.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfprvbqm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/genxwxcpt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fanxiaobao.xyz/Article/details/grvixjbxo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fanxiaobao.xyz/Article/details/gfbuojkob.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxdjgdol.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fanxiaobao.xyz/Article/details/gkauyzbkz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gzzabugqo.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gpwyhpgca.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fanxiaobao.xyz/Article/details/gaqmctozm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwfsspcy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/geiaknkgw.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grmjfuntn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/gchfdipjh.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjozkksw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gclgovnik.sHtML

Go:   if x == nil {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbszchwli.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggicwseos.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyflxdhk.sHtML

[P07] 防抖与节流
来源：http://baike.fanxiaobao.xyz/Article/details/gzspnewqj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnazbjrw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifuuhcbs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqdgetuue.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffywkpua.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyiyfdjz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrfvpurg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsusizys.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gauiaafzw.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fanxiaobao.xyz/Article/details/giblgulea.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhiirxgq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjknsdca.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fanxiaobao.xyz/Article/details/geettwjxu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkvvkidp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcaqyvop.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fanxiaobao.xyz/Article/details/goiaztfkk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbngtidq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fanxiaobao.xyz/Article/details/gregonncm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glkaeergf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fanxiaobao.xyz/Article/details/gkcwmbbba.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtluvqpoj.sHtML

[Q01] 创建表
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfjriyoy.sHtML

CREATE TABLE users (
来源：http://www.share.fanxiaobao.xyz/Article/details/gmumvsrcn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkvhqwjw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcfbanan.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fanxiaobao.xyz/Article/details/gdyohzgfz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gogwscyew.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/grdehzwix.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fanxiaobao.xyz/Article/details/goulqcqhr.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbtqynjk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fanxiaobao.xyz/Article/details/gceauvqsd.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaozdwfv.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/gbvzyqwqx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofpgktpl.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gfhfouqvk.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflltchmg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmdbuqcy.sHtML

[Q04] 修改列类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gukvjprcu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvoqxekb.sHtML

[Q05] 重命名列
来源：http://baike.fanxiaobao.xyz/Article/details/gerjsdsjx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbcerpnm.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxnjlwtx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/gjiydsmza.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gwczupeyk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnplfetep.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gxpovajry.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fanxiaobao.xyz/Article/details/gfbeucgwf.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gavavambi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gqquggwne.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrrjdcwa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemuxksoc.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/gibhtnvdx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/gjjxasizb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fanxiaobao.xyz/Article/details/gjakfvymu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxejaumpy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/ggrhdxbpf.sHtML

[Q13] 忽略重复插入
来源：http://baike.fanxiaobao.xyz/Article/details/gvyhujufs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gqvsdiqvd.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gapfnfhxp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gukwbbbhl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gkyorlxnk.sHtML

[Q15] 查询全部
来源：http://blog.fanxiaobao.xyz/Article/details/gzzmrhrdw.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grolhbxys.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvovvpkz.sHtML

SELECT id, name FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyarkaqsv.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwzluyifw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggevzstab.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gyrdapwle.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/grrxlbuaj.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvcvznvp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmirwneud.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gdotanlgl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggodngezq.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpzudzrx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gxtoradsx.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gmntnojbo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbhyrnoe.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/grjirdpis.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtnihuui.sHtML

[Q24] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpzoimdd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/goydaedak.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/galikuaew.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gjawxiweh.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gpxxxkrwu.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/getxtokfm.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuccpjnq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdgpekzxl.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqqsjvzi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gdtlriijk.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/ghszmcrka.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjxvnpfz.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxgsaotk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gigqfgjns.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gsrtuhjds.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxygsnig.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsirqcdkg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxhehaxn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gaetbpmei.sHtML

[Q33] 多列分组
来源：http://3g.fanxiaobao.xyz/Article/details/gbxrfverp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpacoamv.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxjswykm.sHtML

SELECT * FROM (
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoikuycs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrslpurl.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvhcvqsh.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/grayxgmho.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gotrbjolw.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/ggaeffdbv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gaghfuane.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/grqreyejx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/griaubvcj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gzshkljzn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gzdbxnzbf.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gffedglkd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcmrfnhp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgirpkoe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gmihuxqtp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fanxiaobao.xyz/Article/details/gilkxdvsj.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrcucqmi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdtmjqrg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzomdshb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gosrrkbsr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grppzdpzr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsymmtyit.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gnulgrclc.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/goxnfetdo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvblnoesr.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkvlumai.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgclfqjl.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbdmckac.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gmdokqnsd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gqikzeaxb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gitjpgpgh.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gnxlaxmzx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gnoublofv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmchusiox.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexozvofn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gccnrgzjm.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxodurxhy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgkiuxli.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gikugkjba.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/giygxsrkd.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxggwvwoq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcwirlilr.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gtsvrawnj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gnyfvbphp.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gdqxzqqhg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaeqknzz.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/givvvoezm.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gksujicsu.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gruoxadrf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/grzukjftf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gpancrlsc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuvyxaed.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gcvmndbxi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geratsmac.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiekupby.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkomogkvy.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmwdrwul.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqtvqrwz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gxtrmgahr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gglrmsoit.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsinsuynf.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gcgbiwosy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gswhihmre.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gvdxgnbkx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjianxhtm.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwulntyxy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gwskfwbns.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gneetlhiv.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/getefpnhj.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gcbkumxlg.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/guonouhzi.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gwskjkrvd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxgyoxzb.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxbqntmk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbbsnxvj.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gatnbjvzm.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gswpibdrq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqwpplte.sHtML

[Q69] 查看执行计划
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcnmlyll.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcvejncp.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgebwwxq.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytdmfoib.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gioglzhio.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggumuxumq.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gcluclxig.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/girmaqwzk.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/ghgndsqqq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gfhonqzgj.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gxomxhcox.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gejpdpecd.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gknozesjp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gdnypqfjk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gnylsumkx.sHtML


<!-- 参考信息 -->