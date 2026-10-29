代发 wailian999

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gretaagcb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gzswuoatq.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggyrbkjuq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gzjctbhln.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gncyeznbc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gxfzvpfxk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ggoezrqcu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gykurcfxq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gdyrdkich.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gzptqerai.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/giyjkfizx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gxjztqieq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnzauywth.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gyufxjngg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbvtogmwu.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/guxbijwki.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gwanexbwy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gakjaxlhi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/goitkbejg.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gzwunjngv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gahigpgvk.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gnpdfvkim.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gazjsiuqe.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gbryniord.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gondazyik.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/ghlomcaon.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gtpvbwvbf.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gdfclputt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gqncpwbdp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gxvcsjxep.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/glisqlupg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gjltrwwdp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/glodnkeoh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gsbnophku.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gyibpzdap.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gejhvdgyv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gcqjqhoaq.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ghfwntsng.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gcvzopmaw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gbtybqmqj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gxjrtgixn.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/glphoeopn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gkcprjabr.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gojkdzhim.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gbhdbxtwm.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gizhqqyqv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gjksvgonf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/grqsldrrl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gkwnidmag.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gdmbtroqw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gdzkvaqko.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/guvqdsyvf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gombfcqos.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gglfdctqq.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gfodzgfzm.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gmrcwxhqo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/ghunchqtz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gqhzrqvpz.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gyudxmrtg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gvvlebior.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gdfafmcpp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gqibqteaj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gvmxzjdkl.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gmvqybgfb.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gdbrinjtt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gduyymdka.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gjxyyywaa.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/golgcrdjh.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gcpkfholw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grzmctkfy.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gnduhfqlr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gieyhcmyk.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gatdqbyer.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gmcaecnpq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gejqkilzt.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gzfcihqld.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gofnjxdlx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gzrmltxqz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gfshdcwgc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gbsnksfrl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gkdutjalc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/goilkkuvo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gahxvulry.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gwwmktmmz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gmeaghdno.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gwoywdxvc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gilgoiaux.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/grogyxldf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gwqikulbt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gpislncdw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gpnkrwine.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gyzasumwo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gyktkxsfp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gqakncuod.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/guyimnklo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gaohhrukb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gjhmarovj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gzisgcqal.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gxxlribaa.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gubeiwdlc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gdcvuoxoe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdbzsoooq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gshdcdijj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gruyquefn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/glbsqrumm.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/genzbleco.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gwrqnoagd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/geuoumkwe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gogslwoxa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gjmfmsujt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/glauurfrm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/ghlzzrdmc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsuwuzlep.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gdypvljqz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gahauoexq.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/grxoxtjuf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gnupqlyoj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gftdcvwiy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gpjfxzclv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/grqrrdgvv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gmqohhklo.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gqzkrebog.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gajeutexl.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gdmdyuzqn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gclqvcrwt.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gidejacxl.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gbqsdgbsv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gwcmmduhf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/ghknoymmx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gqcsmjpwq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gnjwgphgq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gpczvyllx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gbuhykzpt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gkfgnotui.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gtsszfrlv.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gdhnzgldl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gzwyyisla.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gimgwnwxn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/glzrfzptt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gwqpqezur.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gnpktffus.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gccdenlki.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gpkptgyoe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gtknkgzei.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzoobwmht.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gjmbtvmjd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goyahxjnn.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gnzbngina.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/ggcabhtnx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gvjfsowft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gssbmggzd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gxrqjhsxm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/ggkrixzzq.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gazhlryjm.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gyurjyobc.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gfbzvjmra.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gvntdlrcv.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gksaevpkt.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gtdbquaor.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gylksuxyg.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gyefjcvni.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gndebijvc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/geauizwck.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gaftlrbit.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gqvsjxrkl.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gooivyuat.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gyttusjpa.sHtML

[Q06] 删除列
来源：http://mobile.hesvh.cn/Article/details/gpxpjpale.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gndmaoqpu.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gkshyfjtu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gvnerumfl.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/goqnrpfof.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gpomztdjz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/guyzlxvoh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gbuurwlbj.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gponnvkbf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gqpqmxoag.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gkjzewjbp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gltdblzme.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gdsxawjav.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gslnsmwmw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gcahlvydf.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gogufnjgm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gulhvvnfl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gmmtqndzz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gxcqxgots.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/geckhgsst.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gqcwvddlk.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gultdqraa.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/goedysslw.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/guoqnztcw.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gnshlwvmo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/ggvyjipxh.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwgzeyort.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/ghweukesh.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gogwbfhvo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gzxnadgdj.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gbdanydeo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gjwyrbddh.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gcuedznwf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gelaelcfr.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/geaweszjv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gitddzmni.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gplxfumkq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gdhcwyjgw.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gwinpdpul.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gnazjusll.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gnlwdxlsx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gallirdmq.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gngptmexp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gflqmdnib.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/ggsrxvoeh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmmcafsrm.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gtscsjhph.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gczgbzeqs.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gvvzqraso.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcnnealil.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwnjjjzje.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/grjvycjlx.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gpjbwcikc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/geyfrnamx.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggdgmazkk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gnwzpqvin.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gxkccbqud.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gsugffbqx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gpdyghynf.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/ghdrxqqqs.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/girtyyrwl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/ggqtjaarc.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gnhgmiuyb.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/ghhuvjipj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gcrwdrpjt.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gciacgzar.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gvyqqguxb.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gyhnzpaig.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/guhnduwky.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gmvzpogbn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gqhzovthy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gijtlpzwz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gsypnrjmq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/ggpvpuhpo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/grpgzzorv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gdogjpvhe.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gpenurqqz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gymvnfoad.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gwzttxcwy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gjpynoadd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gvnonisuv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gxwbaggwd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gugbmanhm.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gbfxlhtcc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gfotntlij.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gbihfhsxk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/goxtmlpmt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gaokaxnpf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/glhbwgtvd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/guhsmabct.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gmpqbhgsy.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/ggvikpspk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gqpwwdnvp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/glansptjd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/ggddohnbc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gzbbufcra.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gdxxbieqx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gabwgigsu.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gjlzdfsqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gzdpuapfi.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gbvsfvkip.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gbsfnkvey.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gtdqrwgpu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gpoupytex.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gziivrtem.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gnnxnokdk.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gfzbhpbuh.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.zdbjq.cn/Article/details/grofjsoxm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/goipzcxeg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/ghmvzocro.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gvvnnhqyk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/geikptmhz.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gdosknczs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyriiszgz.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gynkuuyxx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwwnioxgw.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gtwvmfyqp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/guqtdogmh.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gzhnxsmqi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gehembcqs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjjwiuuwi.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gujhgczou.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzmjxrwbb.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gggapcpcx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/grhughvkf.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gzveguzyu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gmgspatuj.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gqxzeitdz.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gzzkjewpp.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gtbwpvxrh.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gcclwywgz.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gthxypdsh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/gndnwhcdi.sHtML


<!-- 参考信息 -->