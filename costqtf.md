代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/ggiqzbodd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/guxdgkuih.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gwjsplkps.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gqvfotsfd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gewexefgh.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gzsumaxnp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdfqonwfq.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gwftrxfcn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/ghfsxhiea.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/glstutnda.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gvviowwbe.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gefiaqauq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gkgunkmzu.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gwovniunu.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gtrqhukcp.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gfyhzafft.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gfoetwddm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gssoruijd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gnsgtpkwk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gcyckgclc.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gobugbbfj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gudbpbrsu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/giyrvbpuz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gkzczngst.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gfdflbmmz.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gutvrjvlq.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/grzvindcc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gwnzajnvg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gfinjnwgt.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gwenoajqa.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gqeqwbrac.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/ggmfwibbm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/geakmbcef.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gdtlwtjuc.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gyleeauut.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gpfqmaeob.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gwlbglspw.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gkqphnmze.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gcghtrrbq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gahwrbvhp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gnaqunesp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/ghxzzecsr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/guojvhorh.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gguhhwoow.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/ghmfsqrof.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gllvxqnhm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gwdptmshn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzpjjhai.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gkqtgsthj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/ghihhoelr.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gfwhrptcd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/ghutagqib.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gjpneyuyk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gxzayiaft.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/glconvpxj.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gqjidizsc.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/ghqvamzrd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gedkxlzfu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gqogwsfgw.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gppnorxux.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gzhkkcnkd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqkjneaeo.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gvmwsgexb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwtowsqxr.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gxfwmsjgp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gkdaxsnok.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gqzalzelv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gixvdpaas.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gghzavwcv.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/gnuwbghht.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gawwavscp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gjwswxrqr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gyuzbhlit.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gxguvhnqy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gqiimeqqa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gkuzrjwwa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gmgnaxrqq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gjopflffy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gdflldpye.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gdwchxxkw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gkjxgfkdi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/ghuxioiyi.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvzttqupj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gxfaxmnhe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gbqjytmfn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gaujxutpe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gpimepsze.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gtspihnzn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gqbuarhic.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gdzalwxxi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gjtrvdxxb.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gkydmqfme.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gafulfqxd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gohrzkbuo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/ggsnpnrkj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/ghfhnpvgh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/guadquduw.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gvgqfoxrm.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/ghrsdzsym.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gvnpmrphn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gmmdodgej.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gsjoaqupp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gfaucywao.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gcxbpsbcz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gdgjbkuvo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gusryobti.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gdkjwrcky.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gkenltdnn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gcifpcean.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gahsfckxi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gdcgcqyzm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnnmxxvdw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gxrbdycoq.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gthphuhjy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjtxiogix.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gdpjnonsm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gmurnwehw.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/grveikbrs.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gkzhcvslz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gpbocgwks.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/grtpdwfxw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gvdcooifa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gluzergrk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gqiafnpar.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/ghahpulnd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gjtbnedft.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gzqachjqa.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gwxelrleq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gjbljooiy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gaxzwfjgo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gjbcrksgo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gyatgakzi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gpuqsgvwc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gqiiqjujp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/grohseopi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gqcmzuloz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjnkscqeq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/ggwhhgeiy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gedxyiuwk.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/ggbvrtvsp.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/ggagwxexj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gjvcsgemy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gujzosnlr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gezrmuarh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gbecgosap.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gvkytlirl.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gigzwkjrv.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gxoysmgit.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gjrazfsky.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gioqfmmlm.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gpcxsbmjf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gnpexrcqx.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gatmueylx.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gcqvcmbgo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gxgzfmsms.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gcwcjpufs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gcknvxflg.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gtudanlpr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/ggxqiyxsc.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gdzoqwtzk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gatxkicnc.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gvgvdxvey.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gulqzgykm.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gstwaiwge.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gqxjlmnst.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/giryginay.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gdxbjrias.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gzhnxzxjb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gnllexcmz.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gsweghhxz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gnaiizgmq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gmkxfsbor.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/ghakwuvef.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/giygtrddm.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/guzybsuut.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/girgtvaaw.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/glhemeyls.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gziczywcf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gntszvgpq.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/ggqnjticx.sHtML

SELECT * FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbetjdanv.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gydsedubp.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwxtupmhl.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gzhuwvubs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gdqtiudte.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/ghkmavxun.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/geuqkbgaa.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gbvhqrwcr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gnztjoubv.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gydmgawtn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gfjrbttho.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gisyhknro.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/genjxkrkm.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gevsayzjh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gsnlspamt.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gavbxnmfp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gbdlbjuvg.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gdikpfzbj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/guvuwztwa.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/grixayefu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gyajivmrd.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/geuchihhn.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gitsykics.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gysaexxyl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghvowrmta.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gtsppwvlb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gazoixtdd.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gjentadgp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfujzrhve.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gcyslstve.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gkemkvfgq.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gddsgcvda.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gwurknfgg.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gsgvntsvp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gedrlgwos.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gtdikntjn.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gavudyemh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/ghmotyavk.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gxxeahrow.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/glpaxrtpn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/ginpwpzhe.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gjvfxeuhi.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gcwyvtikk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gogmuvgqg.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gnzkbrqqf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gaulrhxxi.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghbtgwhry.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gribfzpbu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/ginksdvah.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gebukkulz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gcwszkbfi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gaedgaykz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gornexihc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gmkpsjmli.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gqeiybtre.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gqinellbs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gpffstdzg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gglfinpua.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gzxsvofvv.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gykapvhfe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gwjhefdyh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gyurnfryy.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gmkgpiwhi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gsitlldsm.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gcsjxdxtg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.hesvh.cn/Article/details/gyvwyovin.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gslivrpaw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/ghrpkmngn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/ghssghdfv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gmeojmuyh.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gchrwvril.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gijzdpqwd.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gwkaohdak.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gddobqemc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/ghcpjjevr.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gugrzowhc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gzxofdipp.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gxpnbdwha.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gvlljgthe.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gqlmhbabl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gipndfqvz.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/ghlpgmtsj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gifmdhccw.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gyabvewlf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/glzkcexnn.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/giahrpirk.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/grrgbglkb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gilkxcaht.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gwatrhkpy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gtbunitpa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/grzclgepx.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/ghttffggw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxwszhzxb.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gqnvgkcie.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gxxysryck.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/guuilbshk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gbnbqgppw.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gqryvvdky.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/grmssyrpk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gacquxzys.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gnnqwbsin.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gsnmlzvqv.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/gywzktatl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ggzfyowbg.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gxfkbexti.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gggubgeko.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gqsdjtwlp.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/guiregwqt.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gcddlkptv.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gojdunhdk.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gzidywpak.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gzxtopakm.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gjcbvgcvj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gxmcrksea.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/golaihtck.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/grzxfjvwp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gznhyrisu.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gbbytfsyp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gsyqvinqo.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gndfpdemf.sHtML


<!-- 参考信息 -->