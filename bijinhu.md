代发 wailian999

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gzgxjmjlo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gghihgbrb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/ggepmqnpa.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gahojprcz.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gpbzchgri.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gfvuaijdg.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gdayaitbv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gahualpya.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gmbkzldgw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gqsidpvet.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/grgciquuj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gpewitucq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gvqpckkpu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gqcmsbyav.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gilxmouob.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/giqipqtch.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmgqwfbhf.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gcdfxynlm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grqzcznjg.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/glcinhpow.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/ggydrmtiu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gxpwyzglt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gqttilpyu.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gtbmvdote.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gvmnhimmd.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gijcchvyj.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/giuynbfzk.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gqpisqerq.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gyvsjxyap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gwmexiubr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gpymkakjb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/goyjiaowd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gqywgkppi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdpcyqon.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gkhiavjgy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gufdlkuiy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/glenhetri.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gsteexkay.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gstchvnwv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/geyvdmwcc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gqvmfcurr.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gdbtwxryr.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gordpnitn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gjbzlisww.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gmagefyyd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gtmhtwzsm.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gtfdaahwp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gtikdlnff.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gljxyltay.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/giiantcyz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.hesvh.cn/Article/details/gtdirabut.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gsxkdkfbl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gmwxuqbqw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gmyuvmnlx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkoefletn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gcqfulsma.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/goxspvnug.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gpjwotgjf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gnpyaxcll.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gshlodgre.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gcbaywuuw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gdmhhwfsp.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gyuzffnrx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gdkgohtim.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gnfaphdxe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gllyayimd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/glzfshbyn.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gwatvgtqx.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gcoyttwqn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gwomytowg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gzihhsukj.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/grdygjpqc.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gjucdrdxl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghviwdaxr.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gkzekpruq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxniaakdr.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gdjvoukhm.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/griesppaf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/glnhkxrgo.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/glexbuhzb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/ggypjomhq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gplfomrzc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gpyigpmrr.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gyrgbucvh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gltlgzkre.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/glafrcxgc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/giigtydig.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gclddwkis.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/goxsfrxfb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gpbqdkxsx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gvlktfgik.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gtmzndoxo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gisysogee.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gdnzmieeb.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gvwvdicqw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gvskqurkf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gztwuosac.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gxahlkhty.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gvwvyyadh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gbajnlrme.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gyymhkhhh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gyinegnul.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gsoanvwmm.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gzifrooxy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gucoourvq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gexjksfsc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gktnecmbr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gfuevmgrz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gmsnfkbay.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkbeodw.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gjawxubsh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gsuzufrxh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gvnckmvtr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gaeuslzsq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/grybtrvcz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gzpeczwgb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gsfwkneyn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gqwthqavw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gjgzmdvfn.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/guozawjyy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/ginruptnn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gplpfnxld.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gmjtnmpgu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gbtevjqnc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gxtrbkxwj.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gkeiqbrmw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ghvrrfxqd.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gwpbbyzxj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gvjdrcosh.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gqnocpumw.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gskpbbgwl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gqcosucqe.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gnbaxymbk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gwpcwdvbr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gxnhzhrcr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gwczuhxph.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/grdivyetb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gwbfzfuxc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gpkcsgmew.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gxkfprmwg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/grmlhaytj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gktnkbzth.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gwayfdizv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gpccpyifu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gbwtwlnlx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/glmkhbxmf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gwsazzmzo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gwvjztznh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdjcozkni.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gjfzycpcq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwwhwhxlg.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gsrtvhnsc.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gvogbgypx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gjzejqvoc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gdckocgjs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gcgcganxd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gxxxeqlbn.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/glknbsfaw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gsysolisd.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/grqoucuzx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gnryhlnmr.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gyykeddtr.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gerjelnxa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/grieebxax.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/glfilfwvq.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gaifkktlt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gkcmbaivi.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gjwupjstw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmkkymsck.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gwugkmpek.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gupzwjfwx.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gbeylqluv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/glsqpntzm.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gikbzahno.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpieccgpl.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gqrtlwppc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gguayxgyf.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gkqpnoplz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ghiawkzjz.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gfazshscg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gimhfiwhq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gvcqbzsam.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gewjjjvyo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gahgbzdid.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gwnfryyps.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gwvcxjueb.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/glvbdtzsv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/grvlzurag.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gsigbzetn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gqklfxbes.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gptovlids.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gmaltrjyo.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnwcefwmd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/giqdxvpxq.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmgnecvfi.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gyrpuiajg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gegkzolay.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gamdgdekv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gfecjwlem.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gnrvwezzc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gpzmtvhsv.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gspbelkms.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gqotynaja.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gobnbnbne.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gvtedifui.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gbfbczavu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/guynirmsu.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gxqlvoehk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gvzxucjla.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gqsihsqyg.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gelsmenxn.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/grxrkfkav.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gntlihtja.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gzlmovwqp.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gexzqkwil.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gecejsefg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/guisoqxtu.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/grsogtqub.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzgrlaqbd.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gizwacjhf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcxxlayvz.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gkexwvpxf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gxmxbrccx.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/grsknzxbb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/grwyhmbty.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gqglyklwc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gvhzfzsjn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gysbdttca.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gyqiknyju.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gmdeludgj.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/ggruoywyl.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gcczjcwyr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gsjqgwgrq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzviosbju.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gierjtdpa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gqnhflcit.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gpgnhxudp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gkhucixdv.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gixqimhdh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gkwrhmnbu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gkdkfavvo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gpqsshlje.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gkenlnqjx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gnhbppfhz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/guqbebjuq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gtnuxgdbe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gqmecpkgx.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gmurkwrfq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gnrsfvnkj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/guvtoggwj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gmtutixgm.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.zdbjq.cn/Article/details/gxpmluwen.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gwtxtowrt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/glqjshpnz.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gymymrjcr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gjieoqkok.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gpnkumbaq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gsegssvwo.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gbezaqdzk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gxishoiix.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gjgtchguk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/ghpfjxuht.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/guvtronph.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gjtswvnwx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/glvyifobk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gwkmyilwj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gqxipexac.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gkkjajcvt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/grscvmyfv.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gmczisfld.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/grjxdvxpc.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gizvhcaab.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gvwganhim.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gdmddsxfm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gediotcrv.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gjackkjba.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gityqlflg.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gtmxargyz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gdnblaelg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gaouxghqh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gbopxhrfw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gheqxcbiq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/goregnpui.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gznawijia.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvpaoenog.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gbtlbibqy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gxhuwqtkn.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gmbwbddmn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gibtipmsa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gfzifuhsg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gnqplcdqc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbyejxmxf.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gulnuxhga.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdgnycvjk.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gninnpxjw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gyxgmllcr.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gfswwhavq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gbadzybyz.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/glqszxliz.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/ghalewrxf.sHtML


<!-- 参考信息 -->