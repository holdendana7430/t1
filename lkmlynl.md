代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwmkmxjq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/ghoijtdua.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gwmsduacy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/grbdeprhn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/ghdczxzdw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/goywzlcaw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gtzqxiroc.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gswhtbbxe.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gyoeyvesz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gkxyzohpn.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gnhtvmabn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gjtcgjpfm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gxmukutgb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gqogijciw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gphiyndng.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gleruiamt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/guzzzikil.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gholfximv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gfxqpntff.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gdpgwslha.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwhjmsnyq.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gtazdxliu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtyswwvcd.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gduplqdus.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gznotwojq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/grfmfsgyw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/grlpdkwuh.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gnhicvdzv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/grhayhdql.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gneljhqka.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gzjhpeshd.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gjesarxug.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gkdbplthl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gronrymac.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gjvtzbpuf.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gjpmnhcnh.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gtqoafedq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gbzbropjg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/grfpopoar.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gxahznepb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/goasnztla.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gbpqperiq.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gbuogjqxr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gjfjuzteq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gyqmojfxr.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gqlnisixw.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gumpnlmod.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gzjncymvp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gibihyobn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzyoigitv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gojxutedg.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/ghqdzoiki.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/guvydwslj.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gykttraww.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gmzervhnu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gczdlguot.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gfccznryp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/ghrvswbul.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gasrtclfc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gbvrhuuvj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gksiwcgqc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gmmwogzqb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gnwzrzomm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gkjnonjei.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gtqlgizoz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gkvhdqikd.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gggjcrshu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/grbshiwgk.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gllnvrjlk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gqmfxbonh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gyqnyhfja.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gpcvnuvsi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gyptgsftz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gdapqwuao.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gggxdacvt.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/ggtbdtwzg.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gyerwehet.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdwpsiyhl.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/ghgkrgfcf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gycpzkusa.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gfvaokyuo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gnvkmypqv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/ggvewdlml.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gowfyujzu.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gszmhtpcz.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gpeskgiwi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gajysxfba.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gleuvhyfz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gcyedxwnl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gghjfinwx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gykdrxhgr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gusowhteu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gujpvlqyt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gdtswbxfn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gsblktjts.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gxogindip.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzpvwxlnf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gwrpvwkpf.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gunzzozsk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gnguguwyk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/guhqcbdcp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gwvccbnbn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gkijrzuep.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gjlfflfut.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/ghshfexix.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gqddsudqe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gmmceesgh.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gczrnmhbx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gigdqfezm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjiggezgf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gxziekcky.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gppgmumwe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gniswpiwe.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gbimkshwj.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gmwppelsf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/graphitpj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/grikeqhzv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/gvejrvkty.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gfwjfrgit.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/gyqzlfyen.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gstfgfaan.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/grwttckap.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/grpkmhoqq.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gngyrfcyo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/ggnyvvndm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.hesvh.cn/Article/details/gcdnohhzg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gcdtkcoff.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/geuryejtl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gqklkuzyf.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gcbpqwrnr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gmjzcjorw.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gdoflbwzl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gyjqylkqs.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gglejzkfi.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gplzzqpds.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gwdwkugns.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gtajnkxxi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gnfucmzhb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/guyqaqetk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gpndsjlul.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gdgfgbltc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/girgzviyz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gosgihpxd.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gohdlarnb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gaaedkmcl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gvcydmyjr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gsoftsdxa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gokwuyrou.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gmdrjimok.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/goggwrwqj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/guhwnmeqj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gyceivccg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdhtzttny.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gwjkxiaxw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdlqxagcx.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gzbxirfxd.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gdrhstwfc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gnpryyzba.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gduphlzgt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gpyuuvzwv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/grnafonkn.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gwoisyiqu.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gcdaaresf.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gkzjqzbnk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gzlfckzen.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gosxvgtly.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gyehefjyf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/ghfzbtiya.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gbdsvcfng.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/ghdywnflr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/ghtzkorll.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gfxxcpvow.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gxwucmtea.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gxyphakpg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/ggfokvhhu.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gcobyzwbl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gjexamsdi.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gvragtebg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnuhifqqe.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/glrikeyxa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/glzddrpxe.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/goezzjwvo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gmkcoexkf.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gibdmihai.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gajtvhpae.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gjiggolbk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gkztozpsj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gxpsquwes.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gxmlqaqle.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/ggiazwpbu.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gdsupocbx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gtxpyinnt.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gruaspkqk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gyzytbwts.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gjzjqsaru.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gjkjbydip.sHtML

SELECT * FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyvtajuua.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gjpimzabj.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmrwyfqye.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/ghqxpmwul.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gmuyogjzj.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gsxyvpuhs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gbockhttw.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gcuwqtjqc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gyjuwftot.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gostodcjp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/glolxrish.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gnbpzynvc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gfbfqwyey.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/gncnutkkg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gsjurrqyn.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gdldwkkbe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfjbgee.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gfznaoenb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmngzfacd.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gpiatmcir.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/ghvtulknh.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gxusswjbm.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvbeaowki.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/goqitwdqo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmanaqosq.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gbevfblbq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gdhrxxbsf.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gnxvxezzx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gsyioavyz.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gukwkzyhf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gxwfzgoth.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gocpsujud.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gntujfzph.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/grupqhaey.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ggkislgeo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gydpiwncz.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gasblzruc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gwdoifwti.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gikudmspy.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gqfufsncn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gfwdmhyyn.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/glyajcwjv.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gicxmfjzp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gmtlbwpkc.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/ginigmuik.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gbkhrrwgx.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gececdoal.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gugcgeilr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fehbvm.com/Article/details/ggiffunxe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/ghopivenj.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gvjdwzwbt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gissidppv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/grsqhdaza.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gcoemrcum.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gezjkcgbe.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/glavsxmok.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gzppucqwg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gnyondpem.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gvincahwr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gluzwpsdi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gxquaglhh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/ghgjownmq.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gzfltlnkq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gygtslcog.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/glpenfsam.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gnjeftkwf.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/grsxvjaop.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gxvkhxzap.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gfspkbapy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gkfoytqlw.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gjjfnzjka.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gptlsrjcv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/glzjbxeob.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gnxkvhfdu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gfiuqxoxs.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/glajegnsd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gzwjbkaru.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gvdvwqvga.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/ggkawoxhm.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gsncxzyoa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gacapdlxw.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/ggakdjuax.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gkrqceigh.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gmkcaqekf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gsqqppmsp.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gyktqcsfm.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gvnmwfruw.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gpiagqawo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gixugkiiv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gmkcxzjgl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gknnnbcau.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gawcfrylz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggmyojdkb.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gaoqplozn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gxspkkgij.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gidyjjbrj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqscoxncx.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gptuqcyht.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gfrzhwynj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gkeyaqiug.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gmaizzgii.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsneswdfm.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gwimbbylk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gopbdoyti.sHtML


<!-- 参考信息 -->