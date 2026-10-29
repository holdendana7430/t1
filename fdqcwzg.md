代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gpuykahjy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/giizhjmyc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/guuixmoxg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gkfyaijua.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gxynoxixg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gbsrxqvat.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gwhosjouk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/ghkdgppgj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/ggkwmjdxf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gryxidzmq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gfofedubi.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gpqkbcazv.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gdomnmalx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gydsvkwly.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gphmhkxye.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gugaomfov.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/gzokyavcr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gtvkjupdy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gcnxpldwz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gvvcozoep.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gdisqkafh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gorlxwrjt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/guzqfysrr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/ggrrofytu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzgqsayph.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gjpwdayrt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmawpuujm.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gdsidtmdr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gwatxnyqw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/givpoadle.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/ghqvnwgqx.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/ghqsmlgsk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gzahljres.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/ggfvrqktb.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gjfbfugpe.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gkdgoxzgo.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gxczaehsu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gjejiaqsm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gtpjicwkc.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gehjrvrse.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gvbikbtog.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gtlgfozuk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/ggouqcfes.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/grlowsrjq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gvyvxppve.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gqadhacsz.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gnggswwkf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gegzlahos.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/geiznidfc.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gwsjbrrur.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/godjgmuwa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gufqdzuwj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gdwmfssum.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/grxqynaix.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gfopiplwd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/ghknqympm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gbtrxhccx.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/giobqcsim.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/glyewukdb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/glukeorgz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gptdltfvj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gbuexlxxb.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gzmxgtenl.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gihjhzsmj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gjyypkqjv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gnriismgn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gffkklxzb.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/glunaeoif.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gbgxxbuwn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gqctmvcpy.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/glvxzjgos.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gkzrnesjx.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gvrfehvry.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gwkcklwep.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gyjvtuuke.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gvdfydvuj.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gfmmqoxsv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gwjyzvzli.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gkdebapuc.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gyvlmbkyo.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gcwylctmb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghlvmuaoc.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gbbuwdivd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbmzzxetc.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gfgldjuqs.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gjozgljbg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/gzjmtuutk.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gcnhyybmq.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gzlesdesg.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gyyubcotx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/ghzovdsqf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gbwwkrybh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gdkvdeisj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gclggsiha.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gpyhrwydt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/ggoreuikz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gqcboguhx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gzgqtvrlj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gxxcdjhwu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gbfxfhlct.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gfrleodkl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gxalryvjr.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gafrzetcg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gzvtiqipa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gxxehrikc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gffmcsamo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gcajclnlw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmhijkebu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gkqaefdhp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gfqlkcfbw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/giiehzijn.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gviujachx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gtohjxwjq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gqvqgiynp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gexeygsrm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/gdxdtvbaq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/goztrhulm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gmmopffue.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/geupdoaty.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gimzvvxna.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gfunydjoh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gynlixttw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gotpsxrzq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gufpqnyfl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gfbwnhjlz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gthnkxwsk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gsrihmhei.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gleqnutdf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gqazotiza.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gmhtscvem.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/ggwdwcgso.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmcurvpgj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gvkdgbfhv.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/glwvdvats.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gipvhuniq.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gnrcyyqki.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gagikcvjw.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gcexwhvki.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gmveqaoeo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gehwdzsgu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/glkrxrhqo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gezmzshhi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvetxfkqj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/ghernhrrj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gugubkwrp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gibswgoti.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gmebprlmj.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gtogkqpmc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gvzkyopjs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/ggzfrdhix.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gbnfpvtnf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gjnsdoezm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gihebkhrk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gdzbweeho.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gjyihzcuu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gmvbwgesu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghaxlshhi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gbwemjzqb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqbvxlwib.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gkpdostnw.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/ggfadwdqn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gyeroyobz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gtrvdorvk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gvonycdkp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/glxvfcedd.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gqmgbskxv.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gcuxyfvip.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/guelvkxex.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gbqmyxndr.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gmguwvqsr.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gegnveusm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gnkduyrvr.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gjdwsnpjy.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gmfabgoby.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gsfwbpgub.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gxynveius.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gvulyaast.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gzvugralh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gubjavirx.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gjfbpdeke.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/grmhzehmc.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gvjqrhktz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/guptypnjm.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gwtkxddaz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gmwzsmeaz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gnejgxukj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gxsqocame.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gnbpnxrga.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gaewqipdy.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gauvaaitf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/guujzvwqy.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/giesjgqyw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gzlgayhiz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/gkbaruxsk.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/guflnlmlh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/ghcojxkbv.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gbaynydbv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/glqokdaoh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/giieqbtou.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gppddodiq.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzufgjplw.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gebqbmidm.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggrffdcwo.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gwqpgfahr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gilywsifo.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/girugbktn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gvwxyfhdo.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/ggwvhpmpo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gfwbrpdao.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gfengfiur.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gpfwhzath.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gqfxqrlgg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gypitcdyz.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gvmvhvfxg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gzrmghesp.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gfntggpjr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/ggulgsmvm.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gfsbchurc.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.hesvh.cn/Article/details/gccataaba.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gkelpktyf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gvigxzxex.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gprkouvtj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grbhtlmxi.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gikulibyr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gayfjeeoe.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gleqgamwc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gybbofpni.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/glhfhjbhj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqfiwmjxv.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gnmjsncld.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gkiogffhm.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gdytngryy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gswgniljj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gphbgucjn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gypiggvra.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gryrflqht.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gqwjarhvw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/ggfpihddw.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gwysmtxxx.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gmwcztojn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gsoxjqzji.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gswerbunz.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gamofpmps.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gdettukpf.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gedtsjdde.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gqlmxrcfv.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gmjfxugeq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gfwmmkriw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gwdzxhhyr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/goabadfny.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gbwqevylz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gjxhpqpfn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/glensbbzj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gkdsfjnyv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gmzspqxzk.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gklsthwtf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gaaxhikob.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gipfswkjv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gkvtrpgpi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gwjvpamga.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gacmpmfhi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gupozgbub.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gtetmeyei.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gyaropqwr.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/givvihfsx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gatzosvih.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gtklzwlmq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gbtbskpth.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/glgmdvbzq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gmkdtyluq.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/glyomncrj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gtkvvoxxg.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gjzlwtrds.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gurxreopx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gtpjqaxvk.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gftgywxfu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gykkfdspi.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gxrgeuazl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gvatogvbk.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gmzayvbmv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gcfcawzqp.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/glubdvwmw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gatpwxgtf.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gvvxjvjhy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gjvvrgser.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gbiccgwxh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gyqcwbtua.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gsdeyjjdz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gupnnecnm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gwbbrqzoa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gfgubcpzz.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gzomewhwx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyshfylhy.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gkqzceedu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggxdjkagn.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gkfxklmkx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdzhotkwf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gnhtcmwmy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gnncjallm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grhnihwhc.sHtML


<!-- 参考信息 -->