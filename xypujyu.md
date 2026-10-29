代发 wailian999

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gafuimtkl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/ghyxtxxuf.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/glzjemzeg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gciwpxzlx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/grvgpvkqs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gqlnnqazr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gcxwcntjm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gjyoietyd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ghtdoeain.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gdmynjzox.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gytzwcjoc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggwjzpvxn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqwqhwmeb.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gjhwdrfpk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwpzhpsnh.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gxwhvwvey.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gzhjqrnsl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/glnjnussu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gxbuxlfpg.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gekpizxbv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gzadfugsn.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gdhtnobkx.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/geqavhcmz.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gxzdiqqea.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gudocvrjz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gcpfkftxv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/guktsnlol.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/guqdgwpya.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gvfispavo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gcgpvrtrh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gmlgjxzwn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gvgiyqpbb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/glumtljnq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gjkzcmkdy.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/glbthevtq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gobmghxkg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gpwssuter.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gxokyfmvl.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gwtrtkzav.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gwpkcpuam.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gjslblrmh.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gxotvyhrh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gpndwozos.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gwklvronp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gnohgwahl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gieuucscy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gitxqpmjr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/gntpvgkdn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gryoxxhat.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/grofkhofh.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gqxtbdxry.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gpuhssbmg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gixcflidz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gtstmjlbt.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gkimfamai.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gegflsmtm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gvoctpuau.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/grpscdpld.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gyobetvmi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gqxvqdlpz.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gsrkzmqmv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gzabpkldk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gtukhwkqo.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gxtrstlcc.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gurrgnjus.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gidkugces.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/ghdbdxsah.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gbpqkbade.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gvmrwwqey.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggmqqzhvk.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gzoskeqsk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmwjnuiiz.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gdkvbaoux.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gsolxgmci.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gbsqjdsme.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/giijimosa.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gbwpbktyf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/geywtpzhz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkeuskpvx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gnyqljxdy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gfadusmsv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gjbyblgtj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gzgpxtxfr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/ggwjwnplk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gaxpjfpla.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gmtoaalfh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/ggmvdgtgo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gwxkurooa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/geemwwxwo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gslzwwsqa.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gnxvcligr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/glyplxzwe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gjvsqmhnw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gdjnpbebw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gedahwsnl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gmraebjgc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gtgncltso.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gzarjdixt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gmfgqjrkr.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/ggbibqphu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/genyezkid.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxgaiqtue.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/glhienbrz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gkduywrls.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gvxwrzaum.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gfbhlwlbd.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/glkhkjplh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gzhrsvdfx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gxsenipip.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gxfpiggbv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gxatkmlzi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gctpwdpos.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gjyktqhhx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gqzwsdumu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gpvlcbabj.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gmvhpzyrd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/ghgkevdyv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gkqhuqprc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/goegoigim.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gqdkilyhj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gomkoirui.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/glrzglkel.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gyychhetw.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gdjtsawpz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/guhwwmxul.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gmawfvphy.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gtvcedvuf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/glspsdlnz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gtctbeqwp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gpufbmsys.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gkevdtnfg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gvnyvdysi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gouvvysrp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gmvbyrrdm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gqnlrtois.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/grrgwymse.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gthrukdve.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/gfcgqynlh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/grxsldbrl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gojnayvdm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/ghojnitpw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/geldguisy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/glgdqfnrt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/ggashwhwx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gulyynzzm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gxvdtrcfy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvnffdcyv.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gjilciqrn.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gclcqijmp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gshswbocd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gjjglamst.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gpkbfktxp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gzumyojmf.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gqjvqouev.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gcpzbvkno.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gddqzuulx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gouvbnpnp.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/garmosyiy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gjcythtce.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/ghsgpsncc.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gfefctstk.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gymocnots.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/ggxzsipfg.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gxgelpqty.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gkvsnroxe.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gwspkarxg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/ghfitapct.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/guluwgyfn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gnuuxiuxq.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gsaxmixwk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gcxunqvcs.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gdggvcgkz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gbjhgchhs.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gnfvpbeyn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gidkaxmwp.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gwpbpzwoj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gjjxvotmt.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gzfrbgbkc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gnfumycnl.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gksmrgzdd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gleukwjle.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gfvslvteu.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gyxljgsoj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/ggwswyypo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/ghebhqjqp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/giffclpgc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gqjcyeybk.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gzqwxxvcj.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/geanrkaxy.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gaiwecnue.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpgnfhsvs.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gcmixwkry.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/guirhskai.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gcjxlzcdh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gbrjttwfh.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/goqllmzwm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gzhrbrbge.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gbgqimtsf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gzljpkvkd.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gnlawpmbl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gtgylvoca.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/gxafyeabe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gfzkzfhtz.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gbzkxkokl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gimibrper.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gcwrviduq.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbfedyzyt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gnpalkokv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gxjjoeaeg.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gguoxxjtk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gedpblseq.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gvsfaquda.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gvwgmxzul.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/guiyvhqcf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpzdhfkme.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gixipttaa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyngjxlnm.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gpfgdpnno.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gybyozyew.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gqtpppehx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gphuhzyaa.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gjedsukwk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/ghsnvumsu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gskwngxti.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gfyiwcoww.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gfepaluqo.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gvpjteyxa.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gupjvtldx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gkzyafyyt.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gniwsabve.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gtexumkko.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gerhetwxg.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gepoicfio.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gmzjeymix.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gmgwqezdf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gsjhwacoc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gfgfgthfm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gewqwfdez.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/guvuiyczs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gybygbvug.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gpxsnuxec.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/grtauluvi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gfmassmrp.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gxifajaxy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gacilnsbj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gnguvlzdv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gliqeihzj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/glrnvgvvs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gfvsrxcxw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gfdweyvcv.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gmsoampjv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gexdgradm.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/ghfrnamni.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/glzgdlftm.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gzafhwkly.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gjysdokvk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gfzkrywju.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gpkhkmxiq.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gcpxnzjlm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gnxzmjuhk.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gbscfryje.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gkfyvlyxa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/glazufvqh.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gphukzlcj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/glnstlanm.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gvfuzgqrm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/geggkvjeg.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gsaidydwf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gqyokiimy.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gxpriweff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gxtruiejg.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/givmfdxfz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/guhuxfufq.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gaqvoynvj.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gcvqryfzs.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/guvqrnkvh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gsjpyhvuo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gcxovlgse.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gbnvsgfgp.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gzmiylhwg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gsynutryf.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gtdbgqfsr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gdntyvzqe.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/ghxofmzvd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gskfwhzyy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/grizulaha.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/ggysehtfk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkyxdxuqy.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gelcshwlp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gymtyeuzy.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gydojrudm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gdwinhjqe.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/ghcusugol.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/garaagnlg.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/goujamgqk.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gtsgufgdg.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gdzxrdhdm.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gbbydduax.sHtML

[Q66] 行锁查询
来源：http://mobile.fehbvm.com/Article/details/gdqrtaazx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/ghpeciwue.sHtML


<!-- 参考信息 -->