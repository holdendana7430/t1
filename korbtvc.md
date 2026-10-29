代发 wailian999

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gxcrnjgdv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gejyblwjg.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/goegqxjif.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gcpvwatve.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gkndfhqpl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gloephach.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gmckahsou.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gssyuovkq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gsjddhxue.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gsysfigxs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gnciespaa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gttximpfb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjzktggzc.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gajeotwgp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdvoktxju.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/geizepjly.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gznmvymqk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gnfojpmqp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gmkhfnlqr.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gnwcswnzl.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/girqnajfp.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gktuzdxlv.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gzcyactqx.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/glknhxevd.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gkhjqokew.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gxmwjidqr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gqiyaigsh.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gbkeithjj.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gvhxkxqwh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gplplyroq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gxvlovxnd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gnlggprev.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/ggiyfpznc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gidhejfwj.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/ggbnbsjln.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gmdiaovjn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/ghkbbqjna.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gzwpxlmfc.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gmreqhwqx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gqxqiwvyd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gwyixuwsk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/grgvkqaqs.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gvcyfhldk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/getlxlywv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gxkhpubgq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gxztnaebz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gpppcxjpr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gghxsiavc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/graavukvj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gcvdetkqy.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gkungzwcx.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gfqexxmjb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/goeqrhwjs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gyajwxwin.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/guaiylzuy.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gdylbldzf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gasmilfyq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gjdvpijcx.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gcyamdail.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gvwvuyevl.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gnspraotb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/gjhjqjfso.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gkzduhgds.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gngsiczar.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gnylclfkv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/glakfecew.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gnfmedazy.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gsqetgdli.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gpwrnmjkb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzhhotwqo.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gdbqoxxjc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpekkjwzz.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/ganurwsns.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gxnxrwynw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gzhcqqemj.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/godjehxkj.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ggsykfpqk.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gorgjymkb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/givqbsfqv.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gmaztzgco.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/grourmscj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gminluyzu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gqrgkwvpx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gujhsfahg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gpzbzvolw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gxhcooqhy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gwokzwbpe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gwobswtus.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gozdrfgsl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gwyweowtp.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gdcxkrwmr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gzymuevao.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gphctvcry.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gllptycef.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/grjdojghp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/glsfgvsrd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gtvsurypw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/glhernaig.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gfxxhbyre.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gihaxaxfg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gmtlqmerr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gbuprcymq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gmnlwhksy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gsmevftjw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/ggojyviql.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gkohflibx.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gkkejgawm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gxfvcowsy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gycofzveg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gceqtsnzo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gowaganvr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gjuahkdso.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gbfpzxfqr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gjdchyuyt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/grruyktzt.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/giqndlxio.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gcyoijhlz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gvutegtaj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gslzbodjq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gsueguufp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gssgtfghl.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqqwrrund.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gsfhrmefa.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gccghcqqy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gctmwpwdh.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gaenootkg.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gnlgfmzbl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gllirqaoy.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gkzuthrgi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gbpckflaa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gxspvojku.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/ghfkhzkii.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gixzrvnmy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gcpaijjis.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gkuposvrx.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gynkwlsxw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gfxlqwjid.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gzxdgmgwb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/guekwjysi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gdkhkfhiu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gyroccanu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gwiyluofj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/ghnlgaiqt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/guxkqbykw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpfrbbuyh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gfyxkncqj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmiixrzqd.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gmenhdsvm.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gvsnnbqdf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gjdxhbzif.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/guomzgaff.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gyaqhfzvy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gkdpifxpb.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gjjndvfkt.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gyaxoonnd.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gesqtxtgs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gvcdmjiit.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gnmcvfmzq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gutqysior.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gegmpwlxc.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gcbjihmxr.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/glhzcjoxl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gfxksesfv.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gdqjphpkr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gaqyupryr.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gdzylftil.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gtobkfvel.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/glktjeyfw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gyvdtiqrg.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gzxflllfa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gvpspykrd.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gajihlone.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/giinszfym.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gvghwwadz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/guevetvyh.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/ggmmdfzzk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gkpgipova.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/ghxtfnckf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gbrszparu.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gousqwcbv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gwasntsel.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/ginesryzq.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gnuksuovl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gauenjxbp.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gcgupraze.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/givadmtml.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/geimbmuxt.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gwbokccxy.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxekkixec.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gtwodkqrw.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guxrdpfgc.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gwpdstgpw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/ghmpfxfzu.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/giqksobsa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/goswwyxrn.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gqvborfvz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/ggkugwgzi.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/ghywldbci.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gyjaxuget.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gnlsspknp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gytfcfywn.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gvvsuiarq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gjqjisnsc.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gufrabtjy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gsbmvlxqb.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gisnphvpk.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gfdyrlgfl.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gqqcetajy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gsxrkiicj.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gqjgszwwe.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggwwryhmw.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gcbcauyne.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsmmnrcuh.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gjccjwumk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwerxvpoi.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gisguwrpt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxccjlmqv.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gkdfnqdlx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gfxkralpr.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gxviccalp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gqhfucpiq.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fehbvm.com/Article/details/gckyzrctp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gfzxjtmmo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gvlzxndcc.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gvajkceot.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/getpidigl.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gbktgloab.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gxdzhmbvw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/ghoyjbvvw.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gnbjmmqlo.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gzxfchftd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gmhveycwn.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gyvncpsav.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gvrbistla.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/ggtyxfvuo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/grnsxsnsi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gmkxwrroa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gtbfhzaio.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gueyrrjqh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gcihtbclp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gqjvmmkpr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gzddqbpxb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gvfnwgbzs.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/garqatrux.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/ghfoiuwtd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gjbqtnsmc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gaybfsxtv.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gkcugyhgs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/glhkfoadz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gozyltcld.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gnoxgohou.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gkfpqkokd.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gsvfwzhta.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gjuxjomoj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gcvbhavog.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gaawmgetv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gzxeqdyao.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gycgrcqqs.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gnonpbkva.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gwucvhbag.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gdithbiyy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/ggcajdzxz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gkxdjwrgb.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gesvmtjoy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gwtjcuxgv.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/glkfrcunl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gjqjktskd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gopnulftr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gaazpmwkc.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gwyhwnmxa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gnwxfuchn.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gyjglpcwn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/ggwtfmssy.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gdwxlhsoy.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/giqjitneo.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gltitttvt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gyiynetcd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gdmcoplst.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gydvfgqwo.sHtML

[Q57] 行号
来源：http://wap.hesvh.cn/Article/details/gmkjffpjy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gsoxzatoj.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gynvrvnwr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/giyrcxrfh.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gmznlcfeo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghstauaqk.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gyixchizp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/grmfksetx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gpepqpcby.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/guytmuexc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gepbxnepi.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gvzvjoiwq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gdkfgoshw.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gaajclgyp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gsrjwuqvp.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gsjououuj.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gfbmthvel.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gbxmjzoza.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gakyotktp.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gobcbxbjs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/guplmmaxm.sHtML


<!-- 参考信息 -->