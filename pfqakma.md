代发 wailian999

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gdeswqwrp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gvjkwijqh.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gapdrjcxs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gqyuvrmee.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gagwwamlj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gkgmfkufb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/glxebwddr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gqwrzmmtr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gpqzegqer.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gxvzilcow.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/givfcuabk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gvhovznms.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnovmgokc.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gdplpkmxn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvkotswqo.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gdnrhgeol.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/geowvmehy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gczwfogoz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gluyetzak.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gtqhmutan.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gwnuubkyj.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gxjagcadk.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gfhmlisko.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gxfkzzlwv.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gvujglahg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gmeonrcjk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gimkgfsfc.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/glodmxwep.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gemljynia.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gidpiyelg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gzpzoqync.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gdygsshvr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gbseiyjgj.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/golzjchip.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gjevyikii.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gzeupfzjt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gilrpfcxl.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gwvptgufk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/giixoorbz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/glrqfyhmc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gvmxddawz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gagwahxqy.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gmporhhby.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gcymswpht.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gagywspwd.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/guzmperjp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gjfuhawfg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gezphdeii.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gjbslvxrn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gfvlkjhmr.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gbodtamty.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/ghpfzvbae.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gsznkaayd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/guqtdeyei.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gtpgptsrc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gsazyzivs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gcquyiics.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gebxhpxsh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/ghtsljfej.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/glwpwvjzw.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gntionnrp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gjwileekc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gsfirduii.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gjohwqipy.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gasnywcqv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gbqawxqge.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gyjygmwcb.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/glxogogeg.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/grbdoxdpd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxxysftbr.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gaacicicj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gievshdhx.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gxjzfotjt.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gjsriletn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gjvpsknoo.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gtmbwbopl.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gzljfqulx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gmbkfcwfx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gwkgbswuh.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gcwbudtif.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/giqvaguif.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gtmktuxyi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/griradrto.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gbnjtzwrd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gwbgvpeit.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gbvaxlehe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/ghilmqmdr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/ggzhdbuvz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gkgiocycu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gycggubqt.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gmwotcbgl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gzichirqi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gkvzoghsf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/geqjoliwv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gnveugieb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gdhwoceix.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gtpgaftsy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gqbmuxlvi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gyopmuton.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gkuaatqiu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gshryumww.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gvqgiqmud.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gbpenddze.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gkvrxrbpl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gkicckvrc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gmxsypriq.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gnnhboljk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gwnusmlgt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gznohyepc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/glueguwkh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gqxqjazdt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gcbipsibr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gmhkwnezw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gjbazyido.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gyobvbwyf.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gdtswffww.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gqonyucpr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/ggeczdbde.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/ggfdvnyzv.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/goguosech.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/guvxtqgwu.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gsbqizdte.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gbfctztuj.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gdmjbiogb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gpmlpeuck.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/garvoadpx.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gueaftryx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gzrvslehn.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gdyukjvze.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gpvpiskyw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gusqcvftu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/ggsamtlbc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/ggabwofmp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gqusfnuqs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gtgxxnvzr.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gspenbbkr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gzzvrntwj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/ggunwmhtx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/ghlvfbuhy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gaksjjlsg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gocdwxqry.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gtqjgxqku.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gwovvcjew.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/glbkyhjby.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gafqltdwp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gzftmngxe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghxgtssun.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gdamghzpn.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/glkljrgjp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gmstqlhvr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/glirthabz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gtligucgj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gjzzkpdgy.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gsbpchnqh.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gjteyggko.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gaeogjqwf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/glrcfoyyd.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gcsmzuanp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gixgrcroo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/ggehpqupo.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gpeoywnem.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/goverdylx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gtsbhcygi.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gvxxbvucw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gbivdgozy.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gpcqmidgl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpkymxpow.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gakhcyubk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gyecswumy.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gmkncospa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gsjjpqbnc.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gwxhbysqp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gvrflqnul.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gagaejthu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gvdlxiqdd.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gwqbkgnhx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gzifrimby.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gldvoiggg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/ggnifwhwq.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gzrzzsmah.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/ghkqahczg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gkcidqkkf.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gnmpiwnfc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gkbsbwphn.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gobjawqlf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gmwytaouk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gnmhslaru.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gggvsskau.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbmnxrwtu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/gnbkhkzhd.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvddscuok.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gtygvaooj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gmzoqmoia.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gvvvrmpxi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gyqgxmmpq.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gdcxqpwrv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gmflckpkx.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gydfuhynq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gmicmvbjd.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/grazyrffj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gntokolba.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gzcygetle.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gkdkjbfzd.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gfxzbvyxz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/goqhiudve.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/ghlscddtj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gzqddmrfc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gbeedqukx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/ghzykexgb.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gkzjrolhh.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwfgnzedw.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gvzmqhhym.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/glqsdtjhf.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gnmwhwgwh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gixorwnau.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gmflipaiw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grpxqyvye.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/ggxnxuxwg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gsuvphais.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gplefvwsj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/ghbykerbh.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/guelbbgei.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gcotqusoi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gjoewhkpy.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gqbawymil.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gidbuoddo.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gnrzqygmw.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gesgessmo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gekasjavi.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gijdagvnj.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gvzogpdyx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ghzgsmcva.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gvmnluicl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/grxfcazsb.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gbqrlugre.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gagzhpalk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gsshavmye.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gtuispoda.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gmtrawzan.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/ganvinkmz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gjzxzakzi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gbwogtezs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gsrcqimhx.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gjnqsfmpf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gdxbiyglz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gtndqziii.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gebzhtayy.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gyadadper.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gyfsvtpno.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/geymzxvcq.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gvuhlognu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gbwyxtxcp.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gmmcvvrjj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gizngvahe.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gvzfpeyvz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gusxnjukg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gomcmqvbi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gcbqvpgmo.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gcleyafwr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gwfbvacpi.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gnxjpbfsm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gnkseilom.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gabwynbcx.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gbfwzhquq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gwzyrecsu.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gijzeltrx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gcujzehlc.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gkwnwkeom.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/grnedexlh.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/grkeuzytf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gwhcnwvzv.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/glrhqeumd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/ghdnlqfka.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gdicrgqcj.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gqjoxqgdb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gmevdiehs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gxkfywuyf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/giuqwaymd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gflmbuhxc.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gmwwaswrb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gpubfbzwh.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gqzusluho.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtjqrwadm.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gieuemvir.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gzhpzecel.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gbinryhjp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gvbgnqcdm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gapkfbcrt.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gmwcgspgf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gamwquqgz.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gbvtfomwf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gtwcowwbe.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gshzudelu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gydpvqzyz.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gnjgtokey.sHtML

COMMIT;
来源：http://blog.fehbvm.com/Article/details/gmjhbyvwb.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gznqwbppv.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gtfxslnqz.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gryfpzosu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gourraoqw.sHtML


<!-- 参考信息 -->