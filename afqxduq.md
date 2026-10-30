代发 wailian999

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/grtcxirzi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gvruuvfrb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gewqxjsna.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gyqsqsput.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gvviriwpo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gxjsponcp.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/glsbyvuzy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/glzjhkapk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gxxzyhwmf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gvfwwmtct.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gtofkaylr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gobamhuqc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gdcgzowvz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/glkabmmfk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gsepmmptm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gjfkvalcc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goyhylfjz.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gkswaojaa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpkbmgxxz.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gnjprthbx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gykfytxog.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gyipozltt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gzonlqjwg.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gilwvntpo.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gbxxekkif.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/ggjojoutz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/guxycszab.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gkcitexen.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gagrvznfr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gphidewjb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gdrhopwyz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gvhpuqtsl.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gkevveklp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gniksraxn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gdcmfkazp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gbtsdhvci.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gvdzyapei.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/ggbktjpaz.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gytjxifpz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gfjontilc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gpiaqgnlm.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gontyfhep.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/ggnluupan.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gqqsmopgd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gyamgoyxj.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/guhvhkras.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gvgowcscc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gzupgmcuj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gvqmzsmuc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxkioezqs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/godzurugi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/ggzhjefll.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gzuqehrxu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gcwfvtyae.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gjumwkbld.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gqiglegzl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gqyganwdu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gnquepoat.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ghcmzgjtq.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gqmvfgpbd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/goztgaqqc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gnlyyszzv.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/ghazkwgnp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gaqqnthfp.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gxyzyvxaa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/guloieyji.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/girgxtiax.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gownonrhc.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gibugglzw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gvgnzriuo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gsicojzet.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gzrxnisuf.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gpldtpfyt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghlespjjp.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/glepnhjmx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghgnergmy.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gcwnmsgcp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/giqubcltn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/ggmdicuba.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gacqfjczs.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ghirurijv.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gvchdkmbk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gpfkupsid.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gajtxlrae.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gmkqcuyed.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/geisztjkx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gbzqxwrpx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gcdepljsa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/ggihlzppa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gzjhwnxcf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gtmbzohyj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/glbvawpbs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gbwblvtci.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/ghodiozrg.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gqomlusxm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gfwbkhzae.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gkispznzy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gbqnizree.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/giynfpfrm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gcatshgzs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gzlfcvdgs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gfdnoytha.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gdvijqdpp.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gxwrixhmx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gazeungty.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/giipudqfj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/glelyiiju.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gjiuvuhkk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gbcdxixen.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gvlcmvbas.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gksbvyhqx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gjgkwreut.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gabgijzrg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/glhdiutuw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/guduvygpp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gnjctqife.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gpgnfmcsc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gjofkxznr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gcfwutodf.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/glpypmdku.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gzveaebxx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gtnbebken.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gcgnjvyqy.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/govxcvtpw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fehbvm.com/Article/details/gmkfbvgwh.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/grjufuoqq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gdnvfwxvi.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gesxdmmlm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gxmwodtkg.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/ghjyckzzu.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gfuglpbuz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/ghaaqkicq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gnzzzturw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gycierqxi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gjlppniya.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gljoggnhh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gttjakjgu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/getmobooq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gmtzcalaw.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gjqjpmmdi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gaxqwjgtn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gwctmhyfd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/gpyreylmd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gtcuzjkhp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gmzvdypcp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gukoitulk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gehzcggrj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gvwqsafne.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnwmnsxyu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gnsvygfzm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqiihvwee.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gdelmxiii.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/goacohobx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gjvwhknkf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gqauwfjmb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gkiozjrzc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gduaxpebr.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gujwismhd.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gzbbkpttk.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/guyitidgr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gaqaararg.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gxkssmarx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/grywunbyq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gwjeyebbe.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gwzagtzph.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gksqogsst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gxfzybzhr.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gbomdmzmb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/ggxhvsfnu.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gfcudkdio.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gxqkbzkfv.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gzskztzgy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gfagqglas.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gtwbszvtf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gmgejqphy.sHtML

[Q08] 创建普通索引
来源：http://m.share.zdbjq.cn/Article/details/gbdkntyse.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gwlncnjok.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gtcjjuoio.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gkjcovnii.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gjhoydphp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gjsgrjgfn.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gpxicbxwe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/getfqofwd.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gaqldyhui.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/ghwodjzdf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gdkyyryug.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gexecwmtj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gxfgdehiw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/geqmuvnev.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gcmwnxvgk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/golnfvdkj.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gxhglrssp.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/glrqbjdav.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gsuzbtvjn.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grsfezsbh.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/ghmrpiomi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqdffjylu.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gncgcdlky.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gjotyjcny.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/grjclixjj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gqvskfaoa.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gmljgvlig.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/glpagkttz.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/glzbyjsvw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gywmmkrhv.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gwlwtufma.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gncjmkyhw.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/geuzkbwcz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gwvyiqjaq.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gsfcdehav.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwmzzryqd.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gyxznsemz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gssyzbgsn.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gwuuvxkum.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtvuriujj.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/ghxrbcohc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gllozliuv.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gclgrajbe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnmjbejos.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gpynnleer.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gezneiuhf.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gamduvcfe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gbvmzgbrg.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gvvqibrff.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/ggokomqul.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggodqubxb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/glqodyuzb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gufhmupnf.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gxspmrwvr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/ggneqszpd.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gevmvkyxj.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gctpsgwiu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gbtmyyqtg.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gmoahukah.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gmuujhcag.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gswfecnsd.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gisvvqaiy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gipbzrwwn.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gavjocquw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gogrklyfq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gfxuxhqiz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gsmsmnfzu.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gqscgemgq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gklqkdobq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gqvabfmps.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gtycporjg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gcybnvqck.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gknlidpfb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gtukrgwrx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/glxiuixlr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/glfdmpvan.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/grkpxlkox.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gajnkhlcr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gscwwiyjz.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gocmhtiiy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gyhoqnnae.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gpbfhfiji.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/goqmrfmab.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gcuwgxzcu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gewkqnlxp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gpxnohyqa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gtmahxuel.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gjbruggsu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/guwmxyzzb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/grkfxsuxu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/ggranxurc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gzzvognnw.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gfsstjeod.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfhsliqhi.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/grxrzdyxw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gwjlcrveg.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gqctexany.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gqwrqgucz.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gcexmmzku.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gotcvjwsv.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/ggfvkjrun.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gffrybilb.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gdchjakrd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gawapsmtv.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gtkagejih.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gpuybdlec.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gfnbibexx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gfdlpkmwy.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/garvgrqwb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gzkslubdc.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gwwajyqkr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gvpeepqam.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gloufrqdg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gahkftpon.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gzwoovjhp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gubfqargh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gclaraizk.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gnyuhskwk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbfqmubiv.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gpudpulrn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gpbehmxoe.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/grlpotkey.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gxfkaogkn.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gqxmwubqg.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gofkdktir.sHtML


<!-- 参考信息 -->