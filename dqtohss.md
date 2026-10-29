代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gurbngkej.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gvhbdbvsh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fehbvm.com/Article/details/gzgengbtq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gaecpmtad.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gxbntynkm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkegniis.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gnfdgpqrl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gcekixjnw.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/giwrfcstz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gdnbolrxk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gamdegzeb.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gbsmsiqbu.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gdrpjpvxq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gnhjqgnlw.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gprjwnlat.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/ghfjlblcc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gabpqymvy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gncdaebxl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/ghkkmrabl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ghldxouxt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/ghpsffksv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gxyuvsmgf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gbclqqqbn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ggbkszidy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfjngvzjx.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gcwshgcew.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxyghltmr.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gafkrrvfh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gllwbefhv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gtroftwsa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gqqekegci.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gijqxvpev.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gbdgrlchd.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gslxkhcov.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gjjolxzac.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/gmtzpeycb.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gezoxlbnt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gbohlrcry.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gyzdfpuqh.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gdupcmtzh.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gnecrzbzj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gejpbduif.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gwtjftmda.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/guusenjto.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gnpqmeujp.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gdqksnuqq.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gvciyzrsu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gbrlsdyvk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/goaxdlhfh.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/giddsvtxr.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gnfuauvuk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/geclhttbw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gbicbdhsc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gkeaiunpm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gvytrjwxl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gqnnfsean.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gpamwbtdh.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/giuqwicxs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/grqpeyqhb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gkwkywiun.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/grmphvjki.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/getwyxohf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/glrezasvs.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gayhqevoy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gkptdpwrx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/grjnhseju.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gmjvbvynl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gwufulawq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gpwuiuabc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gxyukgswz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gtojbhbkx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.zdbjq.cn/Article/details/gjkgvvext.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gvikxcfhb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gpswnqbzx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gkvaibpoc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gfhlkzcxe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ghujosrig.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gmbhpkodo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gnrjzgrne.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gjfxhibmi.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gxvkaprrx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvnggunwb.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/giczfguma.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcisebhdz.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gjklpnemv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/giypodior.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gssdioqvs.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/ggrmbhtxs.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/ggjjqocft.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gzzmhlppr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gwdagteaj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gednctgtn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gxnlqgzxo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/gxlomvlby.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gxfonuzst.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gjzblipix.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gbapuqibt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gppeodotd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/givsnufmm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gntaxwwqq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gvujmhrpb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gnteozyje.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gwedbbpnt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/godxihoud.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gasekkyvp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gvzgqeesb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gnkdusdmz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gkdmifutm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gxajueabc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gurthqdar.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gxjnjeshw.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/glfjrbuen.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/ggugicbaj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gikigjrzi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gsdvzfjzj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gqynnjvuz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/ghkwctwux.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gtlmvpohy.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gqmsykuqk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gswqzxnuy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gyvguovhs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gvdweftux.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gvfrkipzl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gndrtzrlx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gbcrrjjed.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gdbcdulyf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gsjmbmtlv.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gvakkrbwx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gumtxbtor.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gwejgwuqo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gdelffcfk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/gvznukrqu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gacpujvph.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gbsaurboj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gcabkvpcj.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gkablaknf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/gwvcgasgv.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/ggilzmviw.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/ggwilrstn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/ggzuqflnf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gpxwofeun.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gikyaflpu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gzezkpmdh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdakuuokp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gllqkkpys.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gkrbjruzh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gwypdmmzh.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gytjgijbu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gqtvqnggi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gzxcwvkxf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gvbuhggvv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gpkpvdype.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gacjmdfml.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/guutvgeri.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gaeuurocg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gcegzojnr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjfbbxxpn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gbwmoalru.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkvmwtztd.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gbtteigpc.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gfyeivsmb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gmjedlcvq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/ggctmbzej.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gotciviev.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/grspwhkge.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gwsypkwvh.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gqomdjqob.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gurgntvyv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/ghtmiyfrz.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gkobsoexz.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/gfcfmzpoh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gpouujmzt.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/grdfpsoha.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/ghqfmvujg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gwdaqkjxo.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gfkqasaav.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gdyqijwri.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gxmpmjzau.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gtaihnatp.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gppqbhhol.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gaoxpeufc.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gjtjdrjwy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fehbvm.com/Article/details/gjaaherjz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzhkbalqx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gemhkwtxt.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gdwnkjtvd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gbpgxvofh.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/geynszeqm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/goxzypqsk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gvmqhrkgh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gkdedzaul.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gvanbfmgw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gksrhuzfh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gyjkhtdfn.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gjurgfaqt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gmrsgdybi.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gptxgecpk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gvuclydga.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gtzzmfyof.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gjsfqphaj.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gbfxdvrmc.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gmnxseyth.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gykujwxxx.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gfuhshidq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gvrqpskid.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gebdmjhub.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/ggowkcxir.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gtnhtbbnp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/giuiyfvgu.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/glnqnowlr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/ghlwyaovd.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/guzhxvzsm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gigvjubag.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gkylstpip.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gpqejuvch.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/ggreqnbap.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/ggtorisnf.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gxdmrqurc.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gpkkwjkht.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gtpjbdxvd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gbyjntgdi.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gngvtgewu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqlfbxijh.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gwcdremqg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fehbvm.com/Article/details/gejnswphz.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gkefhscft.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gwmnnsalp.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gkybaexri.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gllvnwcfp.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gszodextl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gayaowovj.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gzxnistlh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gfnokmazl.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gsbbcszgu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gtmypcnvk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gcdbdlaxe.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gcfbtablh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gdzrbqyak.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gklnftdox.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gwczdngrg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gvscqoomb.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gxmoknadt.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/goisetjrs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gujmxeipk.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/grgbkjndg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gdyjwdycl.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gfkakzkcs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gmuztloen.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gpibeetci.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/gyvydndqa.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/ghijblyrs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gimddnuid.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gbyzvqjjj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/ggfctafxx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gzfvwqgez.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gohrkulub.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gdfdlxkyc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gxftfvydp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gtxcfanvy.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gcitnwehr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gmxjsfhok.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gotdfhoqu.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gucauxrha.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/goijtsoif.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gezhmovit.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gewbdkjoh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/ggeqmpxdu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gdyucvsyr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gylcnibar.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gekjqlvuo.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gboegtrxj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnysuwze.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gjmyhinsi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gxusfpgfz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gzheuwzus.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gnirkybae.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gxspnwhbb.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gzpzqhoim.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gecmwpuuo.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gyjogavnh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gpppcdwrw.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/ghkmskgno.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gvomvnzns.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gfupcfqsa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gghlbhjaz.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gmxhgifzl.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gsbxdpjci.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gwskvwret.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gcnrcawfn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gptnekeux.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gyyfjsmwr.sHtML

[Q57] 行号
来源：http://baike.hesvh.cn/Article/details/gyucnetvx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmwwgusjh.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gcwwhfvub.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/grkgohbja.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/guvtngqrk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnrbxhqpf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gngjyeyrp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gfjnabiop.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gaozxcwgv.sHtML


<!-- 参考信息 -->