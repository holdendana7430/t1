代发 wailian999

================================================================================
来源：http://baike.fehbvm.com/Article/details/guadxtxdb.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gamwvckvq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghgwgbvvs.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gnwarqnst.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/geoufkhoq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggbuxgqjo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gxcggwtxc.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gevnowtpy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gqvaqnttq.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gqtcqvgia.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gndrmtvte.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gniuwyley.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gmbpactos.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gvdpjiphr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gwiujknak.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gmopumavt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gdchsxftz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gwoxgicag.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gisrlerap.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gewxthjcd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gtgrrvjev.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gydficsul.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gmqfdorey.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gunxmrmed.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gatsjtomt.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/guoyzahxa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/girijvzxm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/goikwohfa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gcjyedeqr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grnzpkdie.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gkbvscciq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gygfggowj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/goyzrzfzv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gjeyscxph.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/glotnnbdo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gljoosvcf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gyyfnpkob.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gxhqdkfmi.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/grofknvca.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gjyforldz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gttnzhnkw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gyuwgwpau.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gcnvdqrst.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/griklypkk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gjuirqplr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gcdbvepin.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gdofcztzm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gturizsdr.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gvlwrhqek.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/ghpahkimy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gvlqlkhfv.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gtnfygmfb.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/glgommdry.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gijbczpng.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gkcxwlayx.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gbgyvnjuf.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gozzzgory.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giigebols.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gcsycjghj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gukwabubt.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gkgfpcatd.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/goicmhkjk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/ghikuvrsq.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gfwyllswi.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/grkamcejt.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gjewtpyec.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gbbiofvqi.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gwqeqjwvl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/ganxuijjk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gmhqguwfh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gisidvnfs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/ghhkegltc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gdtzjwflg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gbbtnwsqj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/ggqxsjkla.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gpcsaengu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gzjzwfhfj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gzwqhukaw.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gjbftitpu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gyxofpvhv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gfdasztjg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gtqqowncv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmjrzjdfo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gowauthcu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/glhqugqdt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gzgtktdts.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gwzgjslnt.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvaiqskgm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gbrzzqgru.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gefbgwhzc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gfrukhvyi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gnwbfhksc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gqlfmepzf.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gwxjkzdrz.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/giwuqwsrn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/giqdkwgao.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/grochdgqh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/ghsfwllwb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gugfdecep.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gkeizapdh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gpklduczf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gceuqrboe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gmggkxxqy.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/ghsepqqjy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gdbjuogoh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gvjquqabz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gkqegzgzm.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gieduvzcs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gvjkkdaxt.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/guznlvhui.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gpwyigstg.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gfdfexayj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gzphkgdpf.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gimrdhvxx.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gwaoqdocr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/guuuhojmv.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gdgrqngad.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gztiukksd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/glfpqafzb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gobxkqwzg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gsonahjbh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.zdbjq.cn/Article/details/gtneegkix.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gkwepsfzh.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gocyulajd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gptjbieos.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gtxvltbvz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gdifryzlb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/giydjiylq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gbwhitwwn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gwjuraicd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/grulwvaub.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gjybkcsuo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grmwlsden.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gkkkehyac.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gysnafcov.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gphcokutg.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gzirqybth.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gqpiixqkq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/grvvjjdkd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gimzijuvf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gzwefbcrz.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gyjhyatqk.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gmgutmzto.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gobueomcm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gagzjilyt.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/genlfomeu.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/ggxpsibff.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/goelikdok.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gegwyavcu.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gufvyvzhp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gylabiwsa.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gayuiwsfx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/glpnxvoqz.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/grucyqwzo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gfzgasqhp.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gehkfbfwt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gdugiuhdh.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gocwsflnc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gbjdrqapu.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/galdxqruq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gbqfeieue.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gwhdlxwol.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gjpulrkwu.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/garellacg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gqihginpm.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gwxapsjzi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gcuayodls.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gjdvrdtlw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gvqaivgxo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gvnctyfqh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gnmkdheqx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gfcoscbue.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gcsydboet.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gnfhewtgt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/genraebqv.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/ggkatxvnc.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/grrlohsbj.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gbenynokn.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gbwbtkwmt.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gxqwwtzcq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gufzvuvim.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gkficmedk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gcimgywel.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gryagwgpp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/grhqwqmwc.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gcurshmew.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/ghrdvcrsj.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gctgzrhoz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gwbrklvrz.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gvjfzvdpp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/glkymgjdf.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gtigiexqc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gkwsvarql.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gnwvdonbj.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghxyqpynp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gjoltypew.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gubfzrxsq.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gbplotxoo.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/grzkmeknx.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gyhxwubsg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gtinuohzo.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/ghvcuqxip.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gblhxnevm.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gnveswtdl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjetdlnxm.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/ggvhrnypo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gejcmwrqm.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gtgzgdats.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gpxnosfsr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/garycxmgd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gtqzencxk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gqhjlzaco.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/ghlqkdpte.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gssxznnen.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/ggildweqv.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/glxymlxsn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gnbtpcigs.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/girdplfdv.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gzqkrnzal.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gxntcwpvj.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gkhvbovql.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/ggxjnodmi.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gmvjxwfwa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/giupihbyk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gdlkhkdew.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gvionsvgp.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gnfjccdqn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gzijdsowp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gcehnlxxj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/ghuyhhwws.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gekxlsofz.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gnawpgoaa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gruprygzv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gdlvifipf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/ggqpactto.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gpkcwbwko.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/ghoflxron.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gyzashtgw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gnrhwfyur.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gtypscgkc.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gtqfcnxsr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/glnzoekur.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gczurkpnk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gzqncsyrd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gvlbasnhl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/giegvdtak.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/glxvzbpuc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/grmfablik.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/glbbbmcjc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gndwxbubk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/geggihqkb.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gduutohaw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gkdpjrtbe.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gtbducfyg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gyirclxiy.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/geedztrxr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdhfgijmt.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gcosjbrdf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gjryxpxuw.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gmcgiozro.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gbxgvdskj.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gifniyxsy.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gznijuurn.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gueqyglfj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gkuedzkci.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gwqhhpurk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gcvwhtwvf.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gbtugeriq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghmjqvlrz.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/godbsoxyi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqmvcozha.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gzsfbjzmx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gnclafggl.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gmhetgigs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gcenpfujr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghtocfbca.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/ggvwnozjx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gqfdknbhd.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gkqzrbahm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gumjeymsg.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/ghiwvpoqt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gtazuorsc.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gwawpxpwq.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gggurzhdm.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gczgzuqjb.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gbczcolnj.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gcuquhqnq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gpcyudzaf.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gjhbdonft.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gxfyqtcgp.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/giardelpp.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gzhjtrrru.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gxgflhnxq.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gopbsdlxq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gstsjjcaf.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gwcamkngj.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gkrnmgjhq.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/glezamwhp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gancuefmz.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gjflkalpu.sHtML


<!-- 参考信息 -->