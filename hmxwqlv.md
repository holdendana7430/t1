代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ghzcckivo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gmanbqzzb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gklurwawb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gkauqtucx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gidtpgvvz.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gtlgqxwlm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzsjznrxc.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gclpmwhib.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gldeyhkxw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnhvjfppm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/goieljzjl.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gsernloyw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gadmtrctq.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gkolxhedj.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/guhraclga.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gtcsqcvuc.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gubzdqkot.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gukqsrfkc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gjkrnxpwx.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gdgcfcrxz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gcbcqjrms.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gatcbflqi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/goomfbphd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gsqomhotq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gyyzbfjgt.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/guacmfyuy.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gebvjgglh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gnnavzbjt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gnilmlkhu.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gmrxgwnis.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghndxxdjn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gpjdvyato.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gmajosybh.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gtgavxgyi.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/ghtdokpip.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/glnamculv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gqbkmykfe.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grazxfcok.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gtlrwnyoz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gicdkaamc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gxsvkmzud.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gwojtvfxj.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gmtqpaavw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/grforcfbo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gxuqtzkif.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gquyubhaq.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gibgavxou.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gaylttztn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gykrlgnlr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gblmjdeqr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gydfwpdrz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gpjoqawmk.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/geepgrsom.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gibkecfrn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gqrfzvecv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gmcmxtxtn.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gjlkbqznn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gvgumhwvd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gnnwqzuga.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gwdjswoso.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gsbwnhvua.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghscgyznj.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gglbgayyu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnjuywvng.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/ghotaffqz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gfzvtttcw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gqobemqtg.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/goyjxznsu.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/glsiekaho.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gmgfkqzrp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gxxlvynht.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/geshiaywq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/guairwkxs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/glvkscifn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gboruhccj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gombyatqr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gqfbvydtw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gntuztimq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gcpeqrfqv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/garsvrrqj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gwwiskhsk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gkyjcnjru.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/ggclajumg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/ggmtspopm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gdhgykhcd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjsanudxk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gpcfzppek.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/ghdkggikc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gktrpajcz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gkrdbgnaq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/goqdqtcrr.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gxkioxjce.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gwmdkhfco.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gtmokronv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gsxkqhvsz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gthxeznde.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/glbphxkay.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gmsesionr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gngbtwlts.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gqrmeitmn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/grlcdiswf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gdyuxdvbh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/ghyfsqdgv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gcvassuvj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gyagpeqdm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gxihxzxyy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/ggtihjdek.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gumagevfl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/ghtatfkpx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gbasagrsj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gzibymvyd.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gkhemdqxo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gnekwtzvy.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gmtwdadop.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gpwxdeisz.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gvbttwjzg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gepbadvlw.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gdqvveigc.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gipnbdgkf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/geghhgfes.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gbrdymuav.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gwrnvhsiq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gzzicdhhe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/glwhhhybz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gupirmdlg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gkzrprkqz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gusyvkkuu.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gbbljgqxa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gwptiyytv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gdrnhlmwj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gceieqvuz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/grphlxbwy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gentigmwx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gpfbcypku.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/godoahvht.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gutobbntj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggknrvnzp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gknpzduek.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gemlewzvg.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gocbcspav.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/ggoxssxst.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gcullreat.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gnqoqnfqv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gkjfcntwr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/grwpfcqad.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gpmzirtqm.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gpnjuvbub.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gerlgfhrt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/grwflkfnj.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gwmkyopoe.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gmzkihwcy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gnibwruzh.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/guvjirdew.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gbzatawnr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gtrzcshta.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/grxakcbhy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/ggchpavam.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gqtepounv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/giumfnpck.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gwrnsirca.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gojxgbrte.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/glknpjgot.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gjzfmrnla.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gxzobmzaz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gevtfzxpt.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/girwokhdj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gxppzifdc.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gpmamyniz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gtkfqyamr.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gianwdcua.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gnzupzaql.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gsqselrmh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/gthvxqztq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gtlmmdays.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gbbwcjvij.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/ggptjpdux.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gflolcmmd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gstmsfadx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gficvmsrj.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gawrnlisz.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gemelmoef.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gsgslnsfs.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmjniacoa.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gsebgglis.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gdkwcqkbq.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gwftuyihf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gxfturqad.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gkbumxucj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/goxjhibla.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gthnopmmk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gqfioegja.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/giyphgqmj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gmztzruyq.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gfzviaytl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gidclbyps.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gofpqyfnk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gyuzwcpjc.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gfgyruwfo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdgazdlff.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/ggxrujusm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gllpqiffr.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gaidnkidc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcbddpyty.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gualwffoo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzsumarcl.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gtrccdozb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glzvkrngj.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/glqwryavy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/giffwruit.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/grwqeolsm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ggmofrvji.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/golgleruw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/glanjcwji.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxavivnaq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gypmcsddz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gtiaymvyy.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gcolnwmia.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/glexkwimt.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gbjmhufae.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/ggxzzbalv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gimtwyydd.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gfcdqixyq.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gziscypal.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gtxaqxrfl.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gnfwjoyvr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gcimycsqo.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gbavftrmx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gnnwkouur.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/giaeqmkkw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gxatmzerb.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gckhkfzea.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/giymbngly.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gffhtuupn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gykrpikjz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gmwmwiddt.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gxqbekoyo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gqoxeohzd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gddvyyvmy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/ghfcollak.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gglglaehz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gxaajjhnw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gwbamqxdm.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gymayzjgy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gzpkxtfnp.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gxizsittf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gijgytkbs.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/goztjlbud.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/girjrkqws.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gcyqnkzcm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/ganrjquvv.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/glbsymyvv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/ghsrzqema.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gpckaayfh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gpzkybwcq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gkxypoxmj.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gfjgljuyf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gwckkcmzw.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gcsgrqcnz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gxmyhbqnp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/glfpynnlx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/guvmkzfls.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/guibczqev.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gsrgjvqxj.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gmcxtapyh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gnshyrtlc.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gvdkahucw.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gzsiquwif.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/glbjcuazc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gftlofwhr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gipwsbbjb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gssebvbhd.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gcepkbnjx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbudohfly.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gfqrxxbca.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gypyovwzm.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gxfgbxkbk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghqitlxtb.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gohylcoar.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gtphewoai.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gqptpneji.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gowjbziun.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjlpetvlg.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gjarhysvd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/glznnwdvt.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gjefbubvj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gjujltgrr.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gbgcnvarm.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gfgwblnuz.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gvthnvapp.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gzjngxdpi.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gyieqrmzc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gsnivoujd.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gsvlkmeax.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/govgmnnsj.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gjzouqkiq.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/ggrsxkily.sHtML

ROLLBACK TO sp1;
来源：http://blog.zdbjq.cn/Article/details/gtwhoajif.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gofzhaccd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gquqzibpn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/guvtaycbl.sHtML


<!-- 参考信息 -->