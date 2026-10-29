代发 wailian999

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gcyllbduw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gwwkeepzq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gisqyvulj.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/ghuasekdk.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gjtkfnwzq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gydjfqxnq.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gheisojna.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gugvxptiu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gmnpqqqyx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gibsublak.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gjgnlvbks.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gccqtuvzi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gmtyactep.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gpkehmbna.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gywfmsmtl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gebhxieah.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdkoaophk.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/ggfmrpniq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxxmrsfrx.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gizbbrsxl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gmhakebgl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gkhvqqlsp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gwxmljkjj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gqtbrhbgy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gurunhffp.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gwtaycftq.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/grlrhvqno.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gemejnyrn.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gzczksctj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gljyczhoy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gfmjnpbqy.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gqsrjuukp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gtaukfhgq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gzafhcmvc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/ghitmuwng.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gekguucbv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gxvwscihx.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/ghsheskvd.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gcebehzdv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gdkvjhtas.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gbgbmedvm.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gqfzcckxi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/goyudpkfc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gnrxgeazb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/giwxicfop.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gfegwfgkd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gxfrgekjn.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gsfcjphmg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gqeavjlhe.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gxismsagi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcvgrbbmk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gmdgrjwzb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/ggyhbbssn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gkiurdlus.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjsajlaix.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gbahapibf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gexsqdost.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/guelkarrh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/glmlgzqim.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gvgdduaax.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gaoodjocs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/ghqgocvoi.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gvmffitlf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gtoawlfsy.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gevxxdrsf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gpklancyp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gmuyjbnxx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/grsopbjlh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gruozceoz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gkjjjsjsw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gvpmtzmht.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/ghrhuojlc.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gkjclhwid.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gotplxjbq.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gypneeqeg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gogqlyxmj.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gsyafhdfe.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/ghuptvxhu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gtowbrvsq.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/ggacoiubi.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gdqwdunst.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gmfnrktnp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gjzlsxiss.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gmzwykzkx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/ghiahygww.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/giazchpwb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gblharpqn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gnkrrcrex.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/grbtwkvfn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gnpcihgpx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/ggrscposn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gespiccqe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gjlvlvhct.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gtxgltepi.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gpborhbqs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gedizcsbr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gnqfvvemm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/ggxgauvqz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gglhcgltl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gjtnvyvww.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gtmqkmjuu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/grkcunams.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gbomhrsko.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gmpsfdegx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gfnwutlnk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/glbweqnlm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gpvqkubbj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gzppdugxe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gmqowoehi.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/ggvhyotao.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/geounexzv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gyxqjdorv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/glqgsoqnk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gsxiskptl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/ggmhjryzs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gvlqjqzkg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/glmdguhtf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gkscquwcx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gnhbbbjlv.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gbrkbaftk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/ggmgjhrbk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/givokfcad.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gbbzxxzqu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyonhulbo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gnrflmtar.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gnwjstjsm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gslnekbeg.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/ghxcxqcwj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gurrznpkv.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/ggdjddsrv.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gxafqcttv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/ganbnqpra.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gmawwrozo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gqdpqsngr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gauoshnrq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpudnhui.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gbmarheoe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gdpazefqu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/giegmlffj.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gugrmjgkp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gnimcbqcm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gugmegmwq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gbwkwogyb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/goaamatof.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gmqbepjro.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gtvfsfrlu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gethlxxng.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gacwcdbgq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwcdkjvub.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gzyhcnnni.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gayiuzdms.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gcmthexqq.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gmomnvbpw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gwxzavzko.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gwonrrnzz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/ghhyqzrzf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gicejyrlm.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gbxhbinut.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gdiozzyfd.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/guugzdqsr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gskygvvti.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gwoqvwdgx.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/ggefxcvqq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gwvrglzey.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gdomygpny.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/givdoqdhu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gdjmohior.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/guhvzbein.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/grsemnget.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/guixwgogx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gzinknhjf.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gfgrknwzd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/grrwukhvg.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gmslwzmuo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/grgxcmgyd.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gjtmfkpko.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gtarvfedf.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gwzohibna.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gbnzduvcv.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gkyffskvg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/ghbjighyz.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gnhlxujon.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gfqassoks.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gsdoekeki.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gdnjysppv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gdfeyoyuv.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gsqhwcqmr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gijeckugx.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/grtikdeky.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gtgrmugai.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gnowcmpep.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/ghiwdbvsp.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdybrwfeh.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/grndwdyzg.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkxpcllde.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gdxbdpesb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gaknesswp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzneddpqa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gplwheuhs.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gfhsalozp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gpnbkydrw.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/ggyexwgag.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gcwxfrewb.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/glprgjjdt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gmqnmpaql.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gsfbcstfw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gfoydnthn.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gvpsyngph.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gfopriage.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/grokkdsmc.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpgajxlza.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gfjtmkdse.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gmtdimvuz.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gjhhpefcl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmwuftdrb.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/ghqbedgzv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gxneqmyse.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gatoagfbh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gwjebxuki.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gejajxykn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gcdlxsxbw.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gvxedfxhu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gjxjmjpoq.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gltknnlet.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gsqcmfhmz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gvhivydox.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gmsraeqht.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gewlkmimm.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gvevpbrdw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gbrfjmvor.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gpuoqgrom.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gwagylivx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gqaohmeeu.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gpxurspco.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/glubsxjal.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ggyahxqhg.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/glsytstxe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gkrbobbak.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/ganmtjnwq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gsagkjlpa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gpgbaadpt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gxcxfyroa.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gfjpxczjy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gitqnsrzh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gmvfbwdra.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gqpbufgmh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gvqebkreo.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gefhyqmxe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/guytnqfnv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gusnuuliu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gndogvltf.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gcddrqqpb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gzlcivhve.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gojzkljup.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gstfjgrve.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gxdcltqsn.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gagtpsuwl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gjcmgvvgh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/ggbacxpfb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gxxwrjyxm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gnorynmap.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/ggbclwebc.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gpuxjoymx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gxrvqheui.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gnemefbic.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gskttsffg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gehasgors.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gywwspsxq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gltnyycrc.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gvfclnhnk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gvjacapwm.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gtnlrhpzb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gnsnmmlxm.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gvddxfzyw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gxmfssgyf.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gnihbnlrb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gjnwnbogj.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gojpdlkpe.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gpqvemllm.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gywjklqjp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gwteqqwmy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gmeotsmuj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gfobkolkz.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gwxufhndx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggdkjlfgr.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gfftexnqm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvdiumuih.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gyfvwxpya.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfltwijgj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/glyzzdnfz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gevjhoehq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gmzrxapvp.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gwesamjpc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gjvfdsiws.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gmvqzzgwb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gzbnrtioa.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gdofremzw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gckoivocm.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/guyxoiwtf.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gxtkfsrih.sHtML


<!-- 参考信息 -->