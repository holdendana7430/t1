代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gemyxqqep.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gnompldrv.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gwbrxoqsd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gvhenzccw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/geujirrgt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gvddsmxxr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gldrzqvxa.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gavvqohoa.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gdbawlkhv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gcpgfxjoq.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gbybcnqhq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gzpeemkwr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gyuzsquoy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gbpedodhj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gbbtzjykc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/girjszlzw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gxsufpqmr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gwqeonsuz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gkwetlzcz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gvqnetydv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggbfbpsgq.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gagxewfem.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggbnojwns.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gytigbrrk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gnrrqvaic.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gvhxxeuun.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gtsgefetu.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gbqxwomwb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gwesybryt.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/ggxxefexc.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/godperxrl.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gxtghxxpc.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gzbyfcfft.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/gzicufrwz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gnjgsyjiz.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gziqjvsis.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gcmwpjbqy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gdpbcnyyd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/giifumnby.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/guwqjpvok.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gzibpxfnf.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/ghoiwgohe.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gbssyxyne.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gwaupguvu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gwhqqrlih.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gggqoghtp.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/grmwolhlg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gphnlbvlw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gotofvhnr.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gimiophqj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/ggeydazyd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gzglzsiuk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gribqflgp.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gcjutqkvp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gpxqzvcnz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gkvbrsegq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gkrnounvh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gyrfcdnjj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsxahcvla.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gjaetsbvf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gemjyptnj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gxnwbvywy.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gkbgntzpx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/golwpixls.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/ghwqiuehe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gazvxczbt.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gumrbbqff.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/glqcljymp.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gubmjwsco.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gtbghjium.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gtbjgdhik.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gmjdcxokq.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gdrjdamgq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gixjzofhg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gwnlttbbg.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gmxoyhpdh.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gblrtrato.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gojpztqgw.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gsomtssqn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gacqhmamq.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/govexmpga.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gvfxiywjr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/glattwgsr.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/garqzjbiz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwfyqriso.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gqzeecngw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gvwulmwau.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/geeddtmoc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gpcsvvsfc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gszhzssjs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gtlddpkce.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/goubikumw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/ggmwnhwzv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gjggshxwh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/guzqkoacj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gelckjcpp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gdqapgafr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gvlegsocu.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gyguqaqkq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/grmzssprr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gqsbhnveh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/goziccojf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gpjuieewz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gqivshxzg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/ggdczdsyf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gfwkmjmvc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gdzhmyjwn.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gjgkbtjxz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gelmxxpwz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grgarxkgn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gzbgvswnz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gfdaijhcl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gicsuwvnq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gdsaglwhm.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gojtyokqw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gdsfgldkp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/ghqbakase.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gltytyfaz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gdsllouub.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gfcbvjiky.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gvnpuxleu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gagpjyspt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gjftbugfc.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gvqzrzlqv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gzyhfhyvd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gduvktjmf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gvtchskaj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gygrsgkhr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gkkktmxhr.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gqxbijrsp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gkeozlqrd.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/ghimlfrpr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gqpfinpbk.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gbclohxxy.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gvjjgsnei.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gftydibgq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gzgcshogd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gnqxhzmuk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gdpccmobp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvmjsjob.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gpkycwqrw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gtggluhvz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gvknjkmyb.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gcufrjjaw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gesgbsfie.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/ggoyticyw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/golsidueu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gmcbyrrfu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gknuceaet.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gziyjgclt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/ghmkbnqmy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gwmytdcyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqaeobiaf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/goruhkufs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbcuppplt.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gkyldthng.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gazqoyxww.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/glbjhgyws.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gwfvgjeno.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gvititbjz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gdoswsjiq.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gzryucigt.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/giozqcmnn.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gfgvojvdr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gdpktvaxa.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/grcylfeyd.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/glfnvkgwu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gepxpujig.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gzzakoezb.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gfoknvmfn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/ggcrnnbxe.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gcsieiali.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gdfxesglr.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gggrgmuxv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/grwytbuqt.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gzqtmhudl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/grbmvinrh.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gzifwwzus.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gkdxkeiux.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gbengenpg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/glqdnkbfn.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gvmfmifde.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gmzbhcvdb.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gctdaoirq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gdhviihqc.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gukitlvpu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gkvgyxkbo.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/ghemwgfdx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gchjzfokx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gtzsfovhk.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gsuczpdll.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gnuzyojdb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gxsjjnlai.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/googscvop.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gwoozcrsm.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gnmxiwhfg.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghkklpkhp.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/grecsuddd.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gwniqmmyd.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/grbpheuue.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gewuechoo.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gfsouuqmt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gsoreyuub.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gszjqbswu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gpwwaoaeu.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gseaczmue.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gwocwuilk.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gldgyxekt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gwmkynbam.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/goydzoghx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gksgtlktl.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gifurqmta.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/ggmjswkft.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gkssimjut.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghqkqzkpj.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gtxtnuszw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gkgettouc.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gnktmvyon.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/genjkpfti.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/glquxiaaa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtdtohxsc.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gyptujcqr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gvbptlrvb.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gpzgkzjsc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gesnkbouv.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/grcrzgyog.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdyaeekdb.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gnkndmizi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gvioajxds.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnrbsmlfp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gonlurhuj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gjqqbibtd.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gceuitpav.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/glybrmuku.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/geqzkckdl.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gynjwrfqo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gbuhmvvgy.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gdffjnxgu.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gmoiogvvk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfrbzljea.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/grnyzpbxq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gkyzcglbo.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gaidqgkeo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gnmfjuwxg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gkhuesfts.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gccitjgxl.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/ghhsofsjc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gniskmlrb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gxjfsspnl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gsbqpylqo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gstbelxnq.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gdnsqnbnu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gmprgvjiu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gzlfreqrd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gldybcvxr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gnjwpbxbz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gtkudrgzr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/guunmhmsd.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gzmicwzds.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gvvsrhnpa.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gixsjudfs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gxbmildpv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gylzsmoob.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gjftnpbvh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gmyyeqmst.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gfzbzuyza.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gjovigbsx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gcgdssmyu.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gwzkbwriw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gqbbzglro.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/giecqvntn.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gioumgumd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/glymeknyh.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gzrctputs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gtsiotgof.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gkijtbjfw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gyfrlrmva.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gkkewdrtt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gzzoqztej.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gufabbisf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gjlsydvji.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gvvdmmuiu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gxhpqblov.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gcsbmirdr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gzvhwmlbo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/ghksqpkxw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/ghkpkolpa.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gjvzxtfgj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gqeavdcjl.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gzvapjraq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gubvtpheq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gdrcwxbov.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gmnjxfelt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gymploqig.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gmtlxfdcg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gfeadulhn.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gcpatojjs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/ggokoqcoj.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gjbiukztq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gbuqvzuxu.sHtML


<!-- 参考信息 -->