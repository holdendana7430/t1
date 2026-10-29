代发 wailian999

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/goyjrtaol.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gfpdzypde.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gokajtuhb.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gqdlshmfx.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grwiilwlx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/geizllpfr.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gbzhhkkjv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gjehcaoqy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gvgozcbwn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gzscvkwkh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gxirktbzj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gpgelfdbt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gglextyob.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/grpcooizi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gbfwkjmno.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gxjogngsx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfozrekyf.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gmslsffvw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtutputjh.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gdsfbialu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gzxolntya.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gbcdjxflh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gayjnteco.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gezagqnif.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gwleibicy.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gqixgwbib.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/ggxtfnxdi.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gajrqceol.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gtwvbppnv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gagqsslev.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gfkdlkpge.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/guglwmpvb.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/girgenwur.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/ggfhknrll.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gfmwqiybi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/giwuasgqb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gqhuqsoec.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gaqubxyvz.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/ghzipgniu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gnnrzzfov.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gdvvmcwxa.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gnultxbfc.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gwlkxezob.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gfrknnbpc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gizzzbofo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/ggjpuctzx.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/guefzqtho.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gmlkvobqf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gmuxytutd.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gclwirdle.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnmlgygys.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/guqloovoo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gdkzraaub.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gaakxjvgf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gqocnbjqc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gmmurwixk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gsypftves.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gmsbjpotf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gotdlqjbn.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gpmycyrys.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gklrwtjns.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/ghwpgqqtu.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gvzhfvioo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gvagxphug.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gttswgjrj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/ggrkbequg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gnbgyjyox.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/ghkcciwho.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gvzasvcgn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gytsxpkwd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gbcfgcnfz.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gnwgyonwf.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gciziosnm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdkyyqemq.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gczlklnux.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfxtbqyuy.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gutcknwlt.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gebpqtobd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gcbtryrva.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gsflzgnro.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gvtudjaaj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gpadzwtbv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gmkjuryzy.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gpbfyuxaa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gfkgbzphp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gufwgjhwt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gdkbwdtbq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/ggrsnyafx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gieiemqpj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gqcpiygvo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gafllpviy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gheoizkau.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/grdidvgdh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gnwkopxxy.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gvdophlgo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/glvytxaln.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gcqcrqyqp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gzstlznmo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gcjvlmlea.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gfdaxjzhe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gunrzuxeu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gfmbpixhx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gblrovqdn.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gasvkbdle.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/ggusiccfw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gfspxwvhx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gdgphorfa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gxoamjkjx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/geoctmkrn.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/ghrzvdctj.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gicvlbydw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gcdrrrhud.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gzzrubinr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gietvsiia.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gvubkvsuo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gvhpteeam.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/grjycdtxo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gnosgdxzq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gujvbrxwf.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/giimagjwj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gkvjpnukh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/grkggzkmm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gspujmejl.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gruxqwicp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/giwngwksz.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gzeusxacj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gfcelnawe.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/geedogvwq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gxmtsehhb.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gsqypxwny.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gmkojwvyf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.zdbjq.cn/Article/details/gvhnblpoi.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gjxndunad.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwfvuinji.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gerczeuyk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gfuglynvp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/giysszrfe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/grbcczqud.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gwbmtdqlp.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gbebroxpc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gnuomstlj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gpwsjwduz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gfuxrvtku.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gxvnyqrcj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/guausmcla.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gezqvrmrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/giyilryit.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gcutpoulg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gohmdnefh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gzmmeyelq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gimxpndor.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gfoimxkok.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gbaiseoii.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gnkbfwyut.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gaxsvglnj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/grxqlcvbj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/ggeegwrqr.sHtML

);
来源：http://baike.fehbvm.com/Article/details/grckcsxoa.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/gzkbuxeyp.sHtML

CREATE TABLE orders (
来源：http://mobile.zdbjq.cn/Article/details/genkxgvhg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gptdnzfnq.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gotsmnzur.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gfmnjtknc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gjndeicyz.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gyuixtccz.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gpydewqmn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/ghwzwbnmn.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/goyncvyps.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gpivoevft.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gjsrfikua.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gdabteibc.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gygzdtchj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gatqqiibl.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gvexnjsgu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gvmcktbnk.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gafqwgsvl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gncxupqmj.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/ggqskfumy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/ghwigxkzd.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gcxnbeduh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/glaujnwnb.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gedwagyzj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gqlovwnxz.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gbbudhnae.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gwjpyttdl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gojkyqvra.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gjxcjpjez.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gvvbemnas.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/golylbqvw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gvgfuzqll.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gflfcacts.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gxtcjeizc.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/grzzxsqoa.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gsqnojelu.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/geyvpobou.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/glxhmyvcq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gelymkvpz.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gnpshpfli.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gkyjdmbwo.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gxwdwqstu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gxhggeycj.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gxwphhlos.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gdczzugjj.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gihcunnbh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gqyhelehb.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gukaaxlfk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gicjynxxz.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/grljqnpmj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gukzjzwfn.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gydgrxfnx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxctggtdo.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/gwbdztaht.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/goxuwxzhw.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/grmnewueu.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gyjhwzmht.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/ghuokvmvd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdglqlagc.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gcaryhaxz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glhppxyuo.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gkoimoicm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gywuqvvac.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gkhtvszxo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/guuqbyiso.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gdibtrgop.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gtvhgksxv.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gcyhpfeeb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gidporlpm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gdvfmptul.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gisfmhsdj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/ghhmduzxn.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/giarhmoly.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/glgotvifo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/grkvedjjr.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gdksxmprn.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gzkvpwdmz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gswltzdas.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gtytpgltc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gjjttbggu.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gvxudyphd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gmlgpuqwe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gfjpvlflx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gayzocrce.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gvfrzxffm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gfhrdvdwb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gxpaouvbu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gojcnxzsi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gddxvmiys.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gvbdsormz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gflasjzus.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gdesvguro.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gpakgsalj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gktadnnup.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gbrekramo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gzwfnhhgx.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gvxbebfaw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gswjznaqq.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gmhryjlhr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gclolqqaa.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gdhtsthdc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/grzvwcvvh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gaxubfoqr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/ghcttdgyc.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gvvlzodwd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gibypohjz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gqqikbwag.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gnosozjff.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gumibizml.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gxgtfwpur.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gwuskfgpr.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gavmxaspf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gzowxjtud.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gjhxxxzmf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gcjaebxbq.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gkwqmqiug.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gbzcwtbvv.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gqltshuei.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/glkexhylr.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gyrrwgnnj.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gxdiobium.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/grxlonval.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gpkdyxuob.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gfazvberv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gvobyudtm.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/goczalrgi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpzoskksi.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gqyucjopu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdhgugsbm.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gcsrsjwez.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gndiwfukw.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gtdrjnidi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gevirhsyh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwrtbuvay.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gzuzlxobz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/goyzvfdzp.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gftvorkpr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/grturdxha.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/glswqhyyk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gavehpzbh.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/geqavexdn.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gholponke.sHtML


<!-- 参考信息 -->