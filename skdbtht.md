代发 wailian999

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gyrjpprvg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gywusynzu.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gjdjfidea.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gxtdpopug.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gktyhgbke.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gonztqvko.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/ggcnptutu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gnuaicdrz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gftkgxiqv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/ggomvidti.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gjogvypht.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gyjcognsn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geblrnhbt.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gxxhdagsx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gschryxez.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gyszympji.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gxnhfppji.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gsagrjsfa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/ggjlcexyg.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ggitgvrqo.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gyegjoycw.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gbsqbgwcf.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gborqciux.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gyapcolbe.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/ghtmaopjz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gzouwgfbb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gjpvauxcf.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gfljboorc.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gzhybgipz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gztndgoks.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gycqlcbsq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gerumbzoa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/grcgslimn.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gstzzhjrf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gncbvxoha.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gryezmdqp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gzcyqficn.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gpvciwqam.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gkmhkbtic.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gmcybmgha.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gtvcldjbx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/ghxckndsg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gmkwvvogp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gmaevunqm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/ghmhzgtgr.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gqcphpwmz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gkbleujmz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gbtspljbi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gtvkrpbkd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gmfpwgtjt.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gunxqovws.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gtrfgvmag.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/ghpvrrzgx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gwvqugibn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gfndnistj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gfvrqyvgu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gturtnbrs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/ghrofbgzx.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/ggpjxlrct.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyuplxfu.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnzxhyoyl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/grzrnpxwy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gxpedxwdv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gitjpfzto.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gvxigehpt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gqkqhmuau.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gkzsccsmm.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gmmzjgzgl.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gugccxznn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbycbhbob.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gpunmpqcp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gctkkmojq.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gdskdjchx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gozmxxsmt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/ggrlaolek.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gnfpwebdp.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/guxfaqwmg.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gvsaxazvx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gofybguhm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gtxlveuvt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gwvevaxlv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gtxvuedyc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gwfbbraep.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/ghkwdsote.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gxwzfyulb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gsrvnvzvl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gtgzxilnw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gipivpjef.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gsihzxvbc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gqpwvexiy.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gnrpouvfw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gyywygwzu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gwzfeozxg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gildfhqup.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gwciwmtnb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gwcjdvnon.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gjqdklspl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gbbhvdugo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gsjgstpdp.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gaizmltfx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gpcxxksqi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gnvpagvvp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/glrixgrga.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/ghcqcxnvn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gzfesivtu.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fehbvm.com/Article/details/gmzuwhsyl.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/grqzrjovv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gpiukkojs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gamirfkvm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gvrxduwjb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gwozdgotb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gugenmnwe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gqfhsgixu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gxyllvoxz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gjgsorwas.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gestopagl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gruvljeyz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gtvaqabtq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gkutthjil.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gtaopauin.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gjblhnlqg.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gzwirzdkk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gdingbowj.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gvvxxbgtm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gpkkuxunb.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyrcmkitd.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gzdjyihti.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gbhzozwxe.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gyupvxbqu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gviivpffo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmqkcaern.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gkapjpblp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/grqenujmg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gvzlmxfsr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gvlvnjbvc.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gfxayhwby.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gairmljvi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gjbeuaxuz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gqsytaibh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gdcgbfegh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/grltszpna.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/giwhhdjfs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gghfqfrlw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gkznzhpbe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtpbvilqt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gxavliwvy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnypsynpp.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gbbbxdqvz.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/ghpouqfaa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gjxecwtmk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/grcanazcf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gnzcjcgxi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/grbkzbinz.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gwmsarede.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gyyywxbkn.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/giovdavvs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gyrauxvip.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gpuimsmpy.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gzwmgsfvu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gfouctaqt.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gdtuokggq.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gitdfdryt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/ggwqubpyu.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gisrdinqy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gfiienqtt.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/guvsuzozz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/goxdpzmws.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gpktmswpx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gjosfadcv.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gjdvnnykl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gfhsmeyer.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gijvehfhu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gwyilzuph.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gutleboxq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gfgarwasr.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/guacdmfeo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gabakagnz.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gehnazdli.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gdxkmgtqa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gvjtukroe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gengkvlww.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/giotqprlm.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gripnruvv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/ghiugxzyv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gwygqwmra.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gxjyzwljh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gdjqruclo.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/ghdchnlfy.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzxbdbvgz.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gbpptlyko.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjuynjkar.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/glqydrrhw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gbqmfzxka.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gtwekbbia.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gvtbobiwg.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gzsktojfs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/gbfuvjgul.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gryscynsb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gygceucbi.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/ghmgnreyh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/guisjsjmf.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gukaeutbc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gdbeghjrr.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gmyulmpvm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gypynbwed.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gisopnzbn.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/guywnmhez.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/ggzrcvhgb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/grxnwlwph.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/glviqxdhy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfjzqrhzn.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/goouglhvh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/goeopwsdf.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gncwvspqc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gniapqxqe.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gxaykdndo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsrcqlzqh.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gmvpdrmmj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/grlfviqyt.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gfwfjkmgz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gllgugjbd.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gtzwfxofb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gxrsgbypn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gufckhqwu.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gpyagpmib.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gfmceupxg.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/glzrxadtg.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gejooxtii.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gowydippg.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gvnsbbunr.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gymscagew.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gnxrffxcq.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/genldavnf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gcqdrfoya.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gagpdyfwa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gicbigtkw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/glyhqidua.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gywujmyad.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/grqwkdqvd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/giefhteyx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/ghqgfipze.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gacpsssdc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gwzyqhngk.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gdhhsdnfr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gumawmjrd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gdbhyppat.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gdsynpmel.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gsjdhblry.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gvyylyzex.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gydozfizh.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/guelwavsy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gxsznecrz.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gdiebsxyo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gascmmwjv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gzqusasvb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gzicnqkjn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/ghvnyanlb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gkasfubqf.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gvfqpazrh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/ggfibrcgm.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gnjmcqonr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gfskuovya.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/glafaxwrb.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gsidroeht.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/geslwidxt.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gosrfzsgd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gktinohkw.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gfqoyakjc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdbdqpmca.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/ghnoceipf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/ggzyjdidq.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gvszpqzlh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gokhuxyjj.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gcieezrsm.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gmbzihvdm.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gavlgtksu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gjbkhtmcb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gconlvlgw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gvvyirjig.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gxzjvamyy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqtackdaf.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gdqrewvmr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gsxdbzkrt.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/ggxpdsjnv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gdlezgofa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gvsvdyazi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gftmeyyzi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/gguhairdq.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/ggmdaezmn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gbzcxdjhg.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/grbbxzhxc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gkbohgatl.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gfbfehxaf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gijhtbfxm.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gjnlnvmwd.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gxeyoavfj.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gjmruqxwk.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gjjavdxxl.sHtML

[Q66] 行锁查询
来源：http://m.share.fehbvm.com/Article/details/gvbkjjzmr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gahkbuolq.sHtML


<!-- 参考信息 -->