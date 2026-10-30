代发 wailian999

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gxtfggtoi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gfpqrejtz.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gfjkgpqkf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/ggfizsrgb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gzmfclpvn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/grpeteoqc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gnyqgmqmw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gkiuagoiv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gxsfvzvsy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/globpkiuw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gaolvdyjt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gnhiswvwe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtlduaaib.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/grtabfmbh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghhuznizo.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/guyhtxlug.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/goiilrrwi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gdsexvyat.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gtoyvbtbb.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gnwcpzlkl.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gvqzhnhot.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gwnjuhxuv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gwdhmzodw.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gujltsnyi.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gypqhqiag.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gvneapara.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gdsgctjuv.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gafszskxg.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/grrvyazlb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gkshqbjkd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gvvsigdxp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gvepsufxp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gcjsuzurq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gqthsehjr.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gzothycky.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gnswmctyn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gqdsiebem.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gasewohfo.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gymrpcbfd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gonbkcwvl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/giiwhuldm.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gvionqbvy.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gxzugypgh.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gmveokbao.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gcxsashza.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gsdlldeyb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gdcukhhdw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gukfovazx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gglefgabp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gquuoxjub.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gklnslzmr.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/guaavxkgj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gunpqdhys.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gpfjrezvf.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gmxiipsxs.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gmfurlwul.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gvogvgxxu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/grkvvhbln.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gdmuxcwcw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gvepljfuv.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gkjprldic.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gwdhjgesz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gmqekmace.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gpznramib.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gdgakpfqd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gdptwewpt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gtbftnuvq.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/greucwiky.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gzcukjhbh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gejydtbww.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gwfrofzke.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcixzfeys.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gsaqiooyd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/guvysqtuu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gtvksides.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gktcmlrvt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gkiwgroya.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gdfxmxues.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gwdzyiuby.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/geimbvpqs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gqifiidqd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gilzkgsjb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/goqbvvycx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/ghewulngp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gomacamkw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/guibupvzj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gozenpzmw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gycfcmraq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/ghaydrpyd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/givsgbnyj.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gocwcmpci.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/grkxcsydu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gdgdkjkyl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gbrdsnfoj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/guvvazrtc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gqgankwis.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gltrzonfl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gvinnamuk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/grlonjhmz.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gllwrqfmx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/glgvwghko.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gjjafezxh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gxfkltfla.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gwodifdyf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gsiahuncf.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gjbzjcaql.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gcxlllsjf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/grlzxpbgq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gagzdrfgm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gpaqsnkvk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gzwxymalj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/ggwynihis.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gnpurlyvu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/guqocjgao.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxbhenzfa.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gozcfbfab.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gmawwhfnv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gibjevopl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/ggtyhtdvk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gibdeqfmf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gnetzolut.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gpjmzrcow.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gqujdrxrz.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/grnnrnsad.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gxfvelhbu.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gvxoszmlb.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gcsoalkzc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/ggzrkbfrx.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gxxaugyab.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gyvbrfnsv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gugwzvtxz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/glxgjwnqu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gonauixyv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gnlvoxhcx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gxydfxuhq.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gpjkqaluo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gqyyjzweb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gyxnehxvy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/glpmqdcnr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gmvnqlyku.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gzdmztadd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gvqqwoswa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gzxyrnkaq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gdldahzom.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwefpmopz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gvwiubytq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkczivler.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gqkmvtgsw.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gppracytf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gmslyqdpc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/ghdnensjx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gbqwzqwwa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/ghtndquey.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/grgzxunyr.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/goimrkdpa.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gehaeqifn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/glhxhapxf.sHtML

user_id INT NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/ghzhupugy.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gwwtgvtab.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gpcfirllo.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gjdarxowd.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gigyicume.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnpgvweb.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gdrzcfped.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gjyqoisvg.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/grtjsyxsg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gdekdzedw.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gdrpltygw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gwwpfpfne.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gohjwppxv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gxikybrsb.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gizdnzskl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gamunamnv.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gwuxtrzzk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gkjhunjrc.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gqncnpovp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gipplsujk.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/giwydgxbp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gknqoyokh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gtldoyyan.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gfycmtoja.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gyedyknsb.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gigauivbh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gisjxovaw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gzrauzjms.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gnaoufqix.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/ghmzyieyi.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gdoxdyhik.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gestwypko.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gomtrmwil.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfjnmzghb.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gzqbpygab.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gazqankgp.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gzitjufhx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gqmaloidh.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gawgyeehb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gwtgkyjza.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gzpjjwovw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gwdvhcllb.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gchegcguo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gngqbtdho.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gxkcrsqeu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gkpneiyyb.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gxmktuzcm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gflfhlqmc.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gxcpamywj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggvzpsdvf.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gtdmujzci.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gzkfxxfof.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gveqnohrr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpalxogck.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gemvxxrjb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmnerfazm.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gvrruwwuw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grgugyieh.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gvplhujuo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gqsqkrrly.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gmcyapstn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gcwowgvwm.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/guowdxwpm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/ghazhhfwg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gsawqapof.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gkbfmakmw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gjttwaeam.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gxvacgfmi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gymsxypsc.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gzluovnml.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gwbuaayne.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gttzpaynz.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/grsyjhalu.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gleiingxd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/golcqxlje.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gcblitpqt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gwbddpgdg.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gtdgnqwwr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gjlckmovm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gjurczvex.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gezdnlxsq.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gkghhajjt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/ghasdocde.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gsreknfme.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gybdniipx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gtzllfcyi.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gllstfhjq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gtfquvwhx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gvlkslbfo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gtffetmtl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gzcdprpbs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/giuocwbwy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/goeanwhnr.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gslwxgyfe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/glqsdlyqa.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gwxnsxtry.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gkwmfmjgl.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gpoxcgyse.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gawmiyfin.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gcvdorgub.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gokmecakh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/giipncosk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gslficbtl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gmmoztnhj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/geyvnqyaj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gmnpyecbd.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gnekjsmdw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gfguhnuqx.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/ghqzyupyt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/ghrkamrdl.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gezoyxxml.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gxzbsmoqx.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gpbnfvuta.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gbtjyxacu.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/ghaaffhmt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/glvwidfgc.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gxgjxtanu.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gululodei.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gersuettx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gzkvlgwhu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gakpkaupg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gsbhhvbrc.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gbqusvwes.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvwdrgxnl.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gqkngasyy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gttmmbjjv.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gockqwhns.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxopxbdtz.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gctuqhsda.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gjxuhhlge.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gahwnovdb.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gkjjwmzcs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggvzmdwxe.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gadefpikg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/goqpwmhyn.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gqqomdgto.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gtfqfslrg.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gfbjrvcwc.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gdchtuhqg.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gcmpaewmq.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gvjnximkw.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gthuoytbf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/geaivfdow.sHtML


<!-- 参考信息 -->