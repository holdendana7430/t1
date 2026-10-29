代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/goffdiprh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gixvrivfy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmqmhqzll.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gcnsxpznj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gxmlbbqbt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gfblvnbza.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gvndmwdxf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gedbdpmoy.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gojnnucxp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gniiziprp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/ghpwgiygk.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/ggzlgpfrl.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gryydnyav.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/grgmozucb.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gxhpeidmk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/giskzffmm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gucywfkmd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/guunvtcua.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gnmucmsnd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gbpvcazos.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/givgszjfr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gfggcdnjk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gfpgoblra.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ghognmbru.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggslifdag.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gklckomxr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcumzrjqm.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gutallpda.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gbelqebjo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gwkqaknxg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gpwyesxrf.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gbdnckuqm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gzpnrflbl.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gpzdwcieb.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gyolgjrib.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gtszfjakh.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gcjohzrpa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/ggtzudtic.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/grphfxmfp.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gehalmcaj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gxwoewjmn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gcwfoihet.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gxdleuivw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gwvsspelq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/grnlixttk.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/ghnzkqvpu.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gfwcerwvn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/goetsxdhn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gmtpbyviu.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gcmtptvbd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gohlnhjzf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gqrhhqdjz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gejsdussg.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gyltoncom.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/ghxeyirfd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gcnqrbrdv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gywbyzbtu.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gpgtzivfe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gmqkzzdwr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gfujvfghg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gpkzlvxlj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gzbixhvyh.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gfsnkuror.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gfesuuyml.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gqqxlcfdf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/ghbvtxbcw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/glkefitee.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gptqqewla.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/ggovgmwlh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/glhprhovl.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gtnlnloon.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/ggkioxjoa.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gfneqbjfb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gvxpqtcen.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/ggelfdcyy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gptlgevkw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/ggqczzjzc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gsuipdkgf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gvbnjeqeg.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gpkgyqupf.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gjfvgchlo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcvyqwlve.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gvpxkfaej.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnoykdvxi.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gxcukiqcp.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gajpqdfru.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gddnyseqh.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gcykkuumv.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gfhxreamv.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gnykhtudi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gqjnvqfmk.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gyvotjttb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/ggmoehnqh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gxwdjhdgt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gdhmlhpyv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/girkpdwdw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gwwcnthxq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gxfkpxzbm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gbsfkhena.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gdzkzfutb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gouafrxcr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gvskkmfvb.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gaiikrctu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/gilwmcxum.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/ggpljeemn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gapkxspci.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/grbgriqmv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gghdljzno.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/grreacfzo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gkbwypqop.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gtluwygif.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gaajxoimc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gltruhzqh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gkoyllbat.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gllnirtbo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gavmiubls.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gupkbhiff.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gtkuicgoa.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/goksizlfn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gxzpppygw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gygkcxlee.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gebcsycto.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gwdxphmrx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gjhzfphzs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gaqfuxvse.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gfwfkseki.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gwkfwptiv.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gdhqupyok.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gigsbpuax.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gnmdiqwhn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/garyyhrnx.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/ghznipmbo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gmcflqzhj.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gsypoaazw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gsrpoajgf.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gcmtoucsu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/glcjbwpau.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/grkbdpvar.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gaitbnkzd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gqhpjifgv.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gvgylsipg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gvvvvcxjf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gspixefyf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gkjuuhisj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gzdjiikdw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gfttduord.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gzbcrvktk.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/glsquwnwz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/goepwwkwc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gajuoulcb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gjxuuxbnj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gfxzffunu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/grxxymtvh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/grqlbyxyx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gqvuuzalf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/ghgfdzgwt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggygmrihc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/gcxfgapvd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjdfrnczf.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gsvxttgca.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gskyxinav.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gwgelxkrz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gswvgzhfg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gjxptqyau.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gaqztinow.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gwigqeyxb.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gsgqvbvol.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gsraaroyn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gjasyhpce.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gwkbvaajm.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gucdtyhzf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/grfcmfvzj.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gcskxxgmx.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gowtosxal.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gskikrdzm.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gtxwabycb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gqgirbctm.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gtvndlbrg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gciykorxg.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gvybkdels.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gsocdstrv.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gcpxlrgcu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gnjxjgxjc.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gamymnnqb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gzhaozsnu.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gdfsaikhr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/geyxhexfx.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gzhniktls.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gyefmflad.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/ghtdixpmm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gpaqbrrya.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.zdbjq.cn/Article/details/gnmcpcnig.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gdcgggfzs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gwnxsnrlv.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gfcoiizud.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gfltjlrdn.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/geokqwxbi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gsniewsup.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gewslnxye.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gvozfmkdp.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsageprwa.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gyxtpifab.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwsttoqrz.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/glqclrhhh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gfbzbvvhb.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gywijrszw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gapcxpska.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/ggmpphvmf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/geswbchlb.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gccicmutz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gdzdrsicm.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gtoovyofo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/glanrddma.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gbptcjwxb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gsmuxnsxz.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gkdsmappu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gmdgtjvxg.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gikuayfmh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbacfqgoc.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/ggyehwajn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gvecooluo.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/givcuzzou.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gixhwryno.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gemexdjjn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcrmwawrs.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gjovxpnra.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/geslxtbxh.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gtjmtlydo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gbpahsuyh.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gguhtscmc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gacvqstpp.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gvmptoarc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/goinpunkh.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gvhaugpgw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gmfombuvs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gmczjmcpi.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gymwmefld.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gmbievqtk.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gihbtskrz.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gvdcixdxx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gldakmbrw.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfiqgqllq.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gubkhxeiw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gnbcjtsjk.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gftcpwjgy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/ghepyzvfe.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gnoiegirp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/grzegniqh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gouegrbcy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/glwycrjev.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.zdbjq.cn/Article/details/glspxcgqe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gerumpgdf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/ghtivtflu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gnttcwxtb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gqwglxxux.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gicykvhks.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gmvzhsxnj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gmywzgedo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gmezimoxj.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gnrxaosek.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gzyxdkmvt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gvrgoruzj.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gwayftjew.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gabbctyot.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gftiommff.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gsljcyfte.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/grahovfxu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gyegmbvlv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gmtfjahng.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/guwhibaog.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gczmpbnvg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gnasictqu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gytaugilr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gdxmqdcfw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gatqvepbd.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gyjybumyy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gfioiaexg.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/glxeofojj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gowymbbeo.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gxazkavzm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gifkcbzjc.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gnnkbzozf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gsqhyxzed.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gbymjylcg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gupargvff.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gcoqxakwn.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gplarbrzp.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gxwexpmgb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gvknupaqx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/glzpjsdvs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gansytbmf.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gxackikof.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gciqfxees.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gqbygqzbc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gqibjbukq.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gdxpvpqzb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gnwalhkil.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gqkivlpcc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gtwelcwwm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvykzlmvg.sHtML


<!-- 参考信息 -->