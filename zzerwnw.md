代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/giyxwqklf.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/ggaaufysf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gypqtcbnu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtujozdli.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gqydezrrz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gouihymmq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/goxlrirnm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gryuelpfd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gtjznykir.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/ghuqwqzhj.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gpvrwstnr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gviquueqp.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gltuvpoax.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gmsrgnxoc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/glrunnlcc.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gllxyyfnp.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gtshxkakk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gpqtupwkw.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gcsvfzplc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gcbdeajzw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gwwqwivgh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gholjxelp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gzzekbbgo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gylxrzttz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gwmhqfick.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gkfaxbfsq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gbfhicjkg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/geoziexft.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnjoephng.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gowvkkfzw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnpsocdhy.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gayzenjnx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/guauwdjtr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gsnpetcmx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gsovoixmu.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gvnpyqbmk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/ghsekpjiq.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gdfjlvpvi.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/georntlfx.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gborykwsk.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gnxzfeiqi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gytkodkio.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/giwqhsvhr.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gzoxxtgek.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gkkbjxvmo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gxbnzzrvz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gzyoyhomt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/geuieyhib.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gtklbakjj.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gldjyzzsm.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggtzbgopa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gsvdyskaw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gsyrsbtli.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gjdnkbkhh.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gxssqrcon.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gawftzigg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gjmsfdioh.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gaafdilbt.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gnpuprfee.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/garwfecps.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gkgmphrsd.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gxnvbkndf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gegvivyzt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gulidprnn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gyakznnot.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/grixjswft.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gnzgpqqoj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gfgjbwpfg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gxjhcyrlz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gsgokipad.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gdoleajgy.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/grgytjqxn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gzxkbgfli.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gavyennnw.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gudrjeeyr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gpemxmpxv.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/ggdxgzbcc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/glnorgupo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gacoptuti.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gobzyeqhu.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gpshfjbsc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gglalutlg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gezxqiihv.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gnbspkouu.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gguakazle.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glpbjmglv.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gqgkjkioq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbdbzpoha.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gcciecduz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/glzlhktgt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gvnwsgijq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gboevdfht.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/grdjopexd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gdrbhmbus.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gyxohbthc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gmyhhaues.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/garkuvgsx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gjabopyew.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/grceibgcm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyuhctnzn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gnnwfblsw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gjobqftuj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gkurpfyhs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gsfcqyhnj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbinumpyd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gytirygzt.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gkfxzucrf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/glbpxkilq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/grqgtubkk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/glmrpmulq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gwsaewzux.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gfegzbazk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gjidiqmqd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gisyzlkiz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/ggrurvplx.sHtML

[P04] 求长度
来源：http://m.share.zdbjq.cn/Article/details/gircfgwtu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gzvsgcind.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxlgkljuw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gshpymhhf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/guetpgpld.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gyllqjjve.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gvyytcfik.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gyjyaosdx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/geyiwyfah.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gwlzozdll.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gbybzbnis.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gdaicrige.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gqifxrbss.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gxuwujmps.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gatkhyafj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gbskuouhu.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/glxekolzd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/goaiswzwr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/gsuoqlppc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gedzalmgn.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gyklhxgkz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gtmfmbboe.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gvrqokaej.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/glwqtcyqb.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gpnasrexc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gewqcsefc.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/glhveoyqg.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gfjvkjnov.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/glkxzshof.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/ghcxqmqte.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gnltaxnms.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gzngjovos.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gndiiieos.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gwsjjgnxk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gogsmjbus.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gzdfrzpih.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gctponuhq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gidpoxliy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gtqdmiozz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gpmayohnl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gcqicvyyw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gttdovlkq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gaocklarl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/glfjrfypy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gcqftjzct.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gekgakdsi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gjhyvhwyx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbqxzkrxx.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gymilycrg.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gfozldtvw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gzjfehsug.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/guddmebel.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gkendwjbh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/grnxbnrku.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gvgkxuuck.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gdzkpdseo.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gpappbcen.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gsxszmbmu.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/ghcihifas.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/gigxkhgof.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gqipmpslv.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gnmcilkqk.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/gkaldptlf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/girjflrck.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gcxyoodzz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gqmixlicp.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gclqzysst.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gwdiujbdc.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/guvupohsc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gopmwqgag.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/glsekgzfp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gussarmgw.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gtqzxmons.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gjdtzzmid.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/guodmklaw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gklbcvstr.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gyhmxtyhk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gwpfywrin.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gxavymjmz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/grdinsbbd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/guemcyoyi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gxnhbwkok.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gwxcfvqjh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/ghxlngwbj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gluyiofuw.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gbrunrnij.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gjetteygy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/ghxjpjgaq.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gugrtaede.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gikmlpiwg.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gyiylkjls.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gohpdcqau.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gmuoapvlv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/ggrzuektk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggsdgzror.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/ghboqjyxy.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gpasxlwrs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gaigphdlx.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gvlvowdci.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gwrnmhhvk.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gguvcuevn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gvvezbacx.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gufsjziay.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/ggpganmdp.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gobwkftcu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gptokmzrf.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/ghnqsqjtl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdwfbkovv.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gmtsdyvmy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/griobtprg.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gbawhodbv.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvodlbpxw.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gsrevepno.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gvxqdqkhc.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gnakurdzw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gaokkphuy.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gglbgecrh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfmjnkvro.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/grgusbgke.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gibiwytjb.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gfwfhktyc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gagkocebg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gmosllshy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gfcnyyiml.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/glxrtnnss.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/geazhxicq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gbhlspiiv.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gyyyotqxi.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/glfuyeoav.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gmabgvkic.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gkaitwqxa.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gtopslufw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gydxxvoqy.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gxkcinbxl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gznlnjxtr.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/glmfkqbts.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gdlkchofd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gjkkludzm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gdnpsexlr.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gtdztiaec.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gcyomgbru.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gvmkkafup.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gpehxqvoe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/guglwvykq.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gjvycolol.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gbudlbjnh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gsgmwpicy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/grbrcagew.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gvamgugjz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gbrfvotyz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gkdfftcto.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gtwaouupt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gwsoiqomz.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gtewmajaj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/girldvohe.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gfgtircay.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gzujhglpe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gvcznrptu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gthitwuqs.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/grcyrueej.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/ghhzaklts.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gahvzrdzr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gkiptxxrj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/glfyjqjur.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/geqnuxgrt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gohyhsflo.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/giermskqy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gbrvikzwl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/grxltcmwb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcuwjodzv.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gvksvpfet.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/giaovmcfj.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gnleqnsbd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/geesmrapn.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/geizjxeyp.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwpyqzo.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gzgvdanrj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gnqdqxkcz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/ghpjpzneg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gzxgheypd.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gvphoeuld.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gptsuwiml.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/glzwjxocc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gfdwyeota.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gnyqanltm.sHtML


<!-- 参考信息 -->