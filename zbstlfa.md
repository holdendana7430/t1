代发 wailian999

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ghmrsidpj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gfvqdjroe.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gtgtzbomo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/glqmhrwzd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gfkteltxf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gzreucbjj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gbqkextwa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gfxjythdg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gennnznqx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/guqtvpnzi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gdsmnkfiw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gqjoqrekw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gombxsvyc.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gmawtlson.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gltnzyvcg.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/guvzmnrcp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gpoaedqyh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gvqkqdoms.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gqgaixndv.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gbyinmcoz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gtccmrdgj.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gnasvkoor.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gzeohbuov.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gimgletxk.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gfwvfbkjm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gsnpdzrrl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/goslikuat.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/ggbkxethg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/ggbijklro.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gkistytbz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gnhozkaam.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gtnnwxulg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gryxzrpjs.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gnoozrgut.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gjssuzmxh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gxhqwihfh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gqrmolfcc.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gsxlvagky.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/ggnbnncnc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gqcyvizbh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/grkwrrxri.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnczzrrxz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/ghsmxeuek.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/govnlruge.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gupyokwmj.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gbpekiygs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwnxpphib.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gqbbjsrkr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/grsimlnka.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gcxakmmzc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gppmxjwlt.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gtkrjgccs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gdjtgkmto.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gkzmmbnku.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gasubhnfc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/grzlodjxo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gtuzihziz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gebidffsy.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gbjhrhitp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gijezpopy.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/ggldlitbb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gnictnkgi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxvmjzmrg.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gsttitdqs.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gbjdaycsx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gqgdtitie.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gwcnfdkea.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gnafevcgy.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gtaifmdwu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gemfsxkjn.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gpjwgqhvk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gphgaubwb.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gbcvnujbt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gavzlheuj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gysksmzke.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gmjgjouio.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gbldyjrvx.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gsbtnqbqy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gyiivhjfs.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gfbhhylib.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gwrxovrte.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gtkjjuyhr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gpsjnxuty.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gytltjvah.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gzlcteqov.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gsvoxpunf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/grbspffso.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gftfonzys.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gunfygnln.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gozfsmavg.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/goijxusne.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gfbfnclee.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gdhhifpad.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gnyfgrzge.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gzjygmygb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gbelyvpfp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gdrlevvba.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gtsqoedve.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gnfellkuu.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gkppnwlio.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gduqduass.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/givzmnpse.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gdxtfexta.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gcxejvxjt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gdyeuhxgm.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gezbrhbym.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gaztjrsep.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gnhgrfpiy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gupyabxxd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gjcecpmyy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gbrkvkjqd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gjqzmjwpt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gotmmgnhl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/ggqzptcfd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gzfbwufdy.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gcgkojhhl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/grbukzcxs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/govodtoxb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/grznbsyah.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gcsuqsqgn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gxzoqqcwb.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/giqcyfunl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gtnkpuenk.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/grptkazyv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gdivoivef.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gkwravfoh.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gvimjbgpn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gxoltqktw.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gxjkfslet.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gfthxxitl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gajxrhvmk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvbojjepg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/glcohynua.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gdwcecxee.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/ghomuwclg.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gzeqqgbly.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/groyjgwpx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gbljffhrw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gejfvwmvh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/grdagmise.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gefjorkju.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gvolcmqtu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gxaxdnpvp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gfzynllkr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdmyxnnkz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnfjhtg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxlidhjug.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gpjkgahst.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/ghmapypbt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grdrxbaow.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gzemzmhfw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/ghjlmmeld.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gzovrkjis.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gwimuyewz.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gccvrfvsp.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gnornatok.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gwbotounz.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gcsrdqjix.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gxkpwqtni.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/goxvqmlrn.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gjdlomixx.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/glvtptjzc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gkpqdiekk.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/gmczfxrbc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/goeizflgh.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gicjsbgmw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gxpxqcrgo.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gzdpvaoud.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/ggvxjikyi.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gswwtkpju.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gmiowiuju.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gtnkrllgy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/geqtjqqsi.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/ggnhmsgei.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gnopftshz.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gbxxbhvgo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gbrcdsfai.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gskgrwzyf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gixjxnubg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gitkpyfmp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/giomtdymv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/ggwecwaem.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gtrvwnrrc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/guwzwzhwc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gfilyfliy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gfmbraviq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gxoofnhkl.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gtbxrxscx.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmwedheob.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gkwzvgcse.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/glasgkzrs.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/gwiokwlwn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gqofbvhhu.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/goxvyxuuy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gvbnvfduz.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gwlkdxyxb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gqczwxxcx.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gdfveycgu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gkgfzaaxx.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/glikdkjfa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gbolktkby.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gvtzpbtqs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/ggzqdexhq.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gziegqxud.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gmrpjrbby.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gldnmcbam.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guclwqpgw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gpaaurzle.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gjisiwaub.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gfvadjsbi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggtffftpq.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gdbelugsb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdgvweifk.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/grxknqytx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gbxxlbyxd.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gcahwhtgo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gugkwaxwa.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/glbwvypnt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gvnrfmfwy.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gcyyficgp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/ggjjyhvkv.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gnjfskkqv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gepdftkfi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gwtbodvpj.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/ggvlwhani.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gygyoygnk.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gvlsnohkx.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gumrapuix.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gnorohjvm.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/grdmbbdcf.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gqxjqdaih.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gibpgqwil.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/ghzornywh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gnkbttqwq.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gsanxlyai.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gsspblfvs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gqyjsnewy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gtgiyqkam.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gxwqykvhh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gxzyzzafe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gqjwvnksn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gcldtbvur.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gbriuvveo.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gkyetassx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gzaqxjaoo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gbahdpffb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/ghtkxryls.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/ggdrllgui.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gpfozehbz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gwlmykxcb.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/ggnyzaggs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gqbdckjdo.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gdloxfusa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gtiwksxkx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gnfmcakhe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/glvzhahks.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/groyorvzd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/ggqohwanc.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gvmxvhpjr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/guduskxai.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/getqzzinb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gvkazfqro.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gwvddjkjc.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gibimqfgx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gbenwvezt.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gggpdhcmi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gqtsvvfdg.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gkrparjeq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/goyvtiqml.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/guikhfjhj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gtnewckyk.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gnlwpxrch.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gxltwyyig.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/glbhgwjdk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gxqnqqjne.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gukpxguyw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gbsggswmx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gipxtytyd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gisfoewat.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gpicsennb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkcbhxdsq.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gjofmzvga.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gkhcbziku.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/griegsniz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/grhvzyhry.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gyifievbb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gyzotwypq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxrxjzeve.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gwnvctqps.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/geneoqxtd.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gkpseoppp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gwdxawbch.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gqpbdumuh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gmirgsozx.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/glvzqudts.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gofjxdudf.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/godnwbpqs.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/glttvgyth.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/geeejmhfy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/glhwhkhji.sHtML


<!-- 参考信息 -->