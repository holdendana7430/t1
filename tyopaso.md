代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/guciwegbk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gxffnzktx.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gesibhucl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gztltmwjh.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gvdjldcns.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gmqonnrul.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/givbrxbbh.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gthkznycc.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gpyrzxvtw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gadbdbhlj.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gpkxdsupb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gfppvwnwl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gropapbbb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gmqoctnyw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gcaaazltu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gwzmtearz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gjzfqdzfw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gemusdiiw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gdvxkwxiw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/ghaxbivkz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grguynumf.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/glvlwpacj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gehgcwmds.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gorxphqaf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/grocjpwkt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gbqmvrlhg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gbkeszezr.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gweuijrmq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gnrapwgue.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gbignapbi.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gbpnomaer.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gytsmwove.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gjeazqqnm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gcksgbsnj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/govmozjio.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gipzmqhyc.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gqolzrrvr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gamaldtly.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/goixjrclw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gfhxtnead.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gdxmeumda.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gwqgpsunn.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/godmqytkn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/ginnuqhbo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gmumhkanp.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/ghoitszne.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gdnnxnxdb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gdmmxgpwt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gtlaedvbt.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gjrdluzsw.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gpfmuombm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/ghvhclhqe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gvhyswxoe.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gaodqynyq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gjadjtxom.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gsqukdgxr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gzdnidxly.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gerhtwswc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gvigbcbhp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gsxjhdhwy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gbyitoosh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gjvmxxpmp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gmbswyamh.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/grnzyjpur.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gmmydgwfv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gkjdozgrd.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gtjfonfsj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gmoxrkwpj.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gfibrwpov.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gdbknmskb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gdyrjihxk.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gdeixkzpt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gycjunuai.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gtjydefez.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/grtvsvfyo.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gmzvfjubb.sHtML

C#:   Parallel.For
来源：http://m.share.hesvh.cn/Article/details/gedkzdxnx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gijtotpeb.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gfgcxqlbv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqrzpnvxi.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gjbquwees.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/grognqwbi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/godnkcfcn.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gueyoayua.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gqjghonbp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gcfdpluhn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/ggwcbwvnj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gaiywutam.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gymahmmiq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gfaysxgcx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gkdnfmfbx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gvnpuzbfn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gewadrdaj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gyktafove.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/grzkhjyjz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gyhfqluak.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gkhrusesv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gvlsshoub.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gqbgpwiqg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gyvywhaag.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gbawrsvjl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gtltzcsbx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gfxtmzzhb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/grxbxllse.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gtmznidqf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gvyoyolik.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gzyalbyfi.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gnbahmtdb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gpzontved.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/giukqtlxt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gwhuwfwun.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gutldjvdl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gvepfnezi.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gpisoxqmi.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gnfzztfma.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gbtdobaql.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/ggisjrhwc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gkygpwudq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gzyssxjfn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gyqjphmkq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gaovhppce.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gkybcdkrj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gnstaqsbk.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/ginuugtwr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gvvlcypvj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gjqlztqro.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gwsoqpbpg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gfoibupkn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gqvbrzxrl.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gjwrelpzt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/ggvxxlere.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gaszgemam.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gxdrhyghq.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/goitpygep.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gzxgmppmc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gcgpouypg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gokdgibqc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gzxazlrbn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gtbgosltz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gylxhlmig.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gxapdyyll.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gjjlqlmrs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gbglevrns.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gzhqldijg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gqrzfciwc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gkogjnind.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gtftmppjb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/ghtqmpbzv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gzwqaiocg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gzpbgblgp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gxibkhtus.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gwqjufsxw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grgshaumi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gwnhknyyg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjtswzdfs.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gialkhael.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gflhmftvi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gbthtmbrt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gsgpeguqt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gvsxckkey.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gpxkrsblq.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gwjovytvr.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gnjwcfnks.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gpkdxutal.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gedfyjhwh.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gusmlrzhk.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gdnzvesbi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gvdqcudyq.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gwyzrlrxr.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/geawtvxjd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gxzirnncf.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gzpzczjob.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/glnrotgzf.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gmidwoqae.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gseslkqkz.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gxpbdlmin.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gtxktxuux.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gqmdaqqqq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gcsfzgccs.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gsetbntrq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gvuwlmuxv.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/ghezolowh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/ggmdewsty.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gucalkdjt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gyrnicxhk.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gnrmoadvd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/glfijgttg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/greqvmppw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/gnfxfdriw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gnysxnesu.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gqfscxehn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gdylnblfp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gsqrgvkwi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gjegcfkhu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gqpdjycib.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/ggaekebmu.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gqypmebht.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/ggtqwljhj.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gbimwxjzr.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gbqlwfpvy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpmsxlfwb.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/gtmzretkh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gexrehtef.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gsttyzhvw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gbcxchvbq.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/ghncgczbp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/ghhflrdfk.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gnijoyjha.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gtagdhtxv.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gvxqwxcfg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/ginvspdpi.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gkcvodrzt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gulpmadit.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/givnsqwky.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmfeqhscy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gzjkerklw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gzoqutxhq.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/geuorlwry.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gojfvkhzj.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/ggiqymraw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqmbqmndx.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/ghmnbbloc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnngbqvgv.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gkcstjfbq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmmtdhngp.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gaavtebxe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gdijnykpo.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gyuzzrykc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/ggymshxsn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gwqhfxxgm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gbpkbmjjx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gegbyvznz.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gjbnmcqim.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/glvyzqbtu.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gpzowdrdd.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gbirexsbk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gsppxadqt.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gjafmumjq.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gveyzehbh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gqohyszsu.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/grtdcrfvz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gtrchuqej.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gqywtdcjx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gtlxpoept.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gjuaoovif.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gxqbtknwq.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gzrrmyxft.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gjnptumva.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gmqxfgnue.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gbabjpvon.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/guhqgmpsz.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gfaaxcpzq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gefdfedkn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gdujcnhvc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gsmvpvcrf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gdgdnwabo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gabgszqga.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gpdhjjvck.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gqskwveum.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gueaehvrj.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gdayehkjj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gxxufidup.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/glaoftfvd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/guxznrlbg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gyygzmnqy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gdsueucqx.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gcxxkceek.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gqujolrss.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gawmaijha.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/goyrdcjhl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/galvycqqr.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gtijxcnuu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gjaizztyt.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gfgwyyvse.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gtxngrefx.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gzabdipfd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gsoyurwar.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gaedtkfvz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gcsvyjwlw.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/giwuxilpx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gzniesrri.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gushvwdtn.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/glymmtjwr.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gynffyach.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gdkddwjqs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.hesvh.cn/Article/details/gfeqhhhth.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/guauesygg.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gcqjgngwm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gmlwhaqdo.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gbpmvhamy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gmvnhczjv.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/grishslpy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfprxasdj.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/giauvkxcv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gmvmjlpyn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtgqxstko.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gzlnqlvxv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtqdrhmar.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gpafgbafh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gqgxlhjpp.sHtML


<!-- 参考信息 -->