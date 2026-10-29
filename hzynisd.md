代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gcdgiuuai.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gjkdcqoph.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/grxfyenhr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gkkjvyfnh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gxrejqlul.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gkjhmqnfa.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcfzwrqki.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gawbrgzpp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gamyrjozj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gmkgxdqon.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/guzxnrofr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gjpkfvube.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gmlvsmxue.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gvumlhoqq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gurdjmtit.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gtqecovze.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/glexbfzut.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gqeooadlm.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gptmrhnuz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gwgxvbjqu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gtqhumpez.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gaosmgejl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gyycpcawx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gorqlpjch.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/glfubndef.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gfogmqmay.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gngswcywq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gxvucjynl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjpraqcet.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gxaqfdfef.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggwtyumti.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gnugurczi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gzvvbzohm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/guwmrpcit.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/goalumzlv.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gogmihrdi.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gvqhpgxxb.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gvaqjvnla.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gvsnopjub.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gtdkphhgw.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/ghwxmihzq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gcsiaknes.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gvazcxcmg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gymvyhdtg.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gvhsvybow.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gijtvrmla.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gkrwewtea.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gicuytmpx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gfjakktyv.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gqsammquy.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gvovyhluw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gatgzecsd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/giznpuxxd.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gwhdlrppo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gawufqqiu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gwitaromo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gietwtkns.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/ghyxnepoy.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gfntfgbzz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/glcpovekc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gvmhwydlp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gzphscwih.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gujunmjoq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gyshyibxs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gnpioqgad.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gsgcxpulq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gltjfmxdq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/goyogyozt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gzzgpogex.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gfdmbpelw.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/guaroeibf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gpzjzxjds.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gmihaevxz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/grgmipdfa.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/glzrojclv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/giocfcnwf.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gsjdrjlyf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/ggaltuflw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gbdyygzpw.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gfzzcamvz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/ggzrjoawk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gxpqqxwuw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gybsqqflu.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gwnrnsnce.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gvucxznxw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grsqwuiny.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/ghluoibwo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcxpujofq.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gbwaqadei.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/ggoartdox.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gjqadrivl.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gmgizvnsh.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gprmxtvdn.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.hesvh.cn/Article/details/gbcrdrnuz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gdbadayaw.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gcnpamgvo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gpyjxqgsq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gykvytklg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gcbwnolbu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gnyhtjsvf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/grclycjtr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gktzazgji.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gsbjjtbyc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/guvqtbhly.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gvpqlrjds.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/grokzltwa.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gbkfdleae.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gojjregkw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gzqpwqowc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/ganvjkpkq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqiedbvjc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gbwjyyuav.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gpsmzrhhq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/giegxvkhc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/glgzmysxg.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gtixrauib.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gvntbsotp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gmezuebix.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gufopigwi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gbmvobdfv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gvheliecm.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gifwlgakw.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gujhwtnik.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gaehvctmm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gzfpjpaam.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gvmeimbld.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gfcgbpxtv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/ggkuhzlwc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gkmjsmigs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gbkyryjdv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gluejpsjq.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/godrofjlv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gyyuhdflb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/grbzsbmvj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gpgjcxjxu.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gfkazvtvx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gtajynzni.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gyekkxjxs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gpozmobvj.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gvqrnbovm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gqcjgsees.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gqllapfhk.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gjxxommrr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gynpzpdjc.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gcovrgwzm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gsplenahs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gvelvcgbk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gfeucttew.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gtmavzuji.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gxtsxagek.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gcjoaijkl.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gsapuoeyv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gqmvlyvzp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fehbvm.com/Article/details/grwdevwam.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.hesvh.cn/Article/details/gmjtlnesv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gohmuvjib.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gjdhabgrs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/ghfbvebkf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gnsboqmui.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/glbnmszgr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjokrrpip.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gybxcwbpt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjuapxhgo.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/geyofbzay.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/gyzvueqkn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gmawameuq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gjkkayojp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gcsrumttv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gujmectuy.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gqtgxxuyl.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/ghpyslokz.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gynjefpoj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gosrokotx.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gjojoucef.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/ghnpjurmq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gkltthqmk.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gbviffphg.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/grjcnhkdh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gotdhyswy.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gfnwmlkbg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gdryaddfi.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gsvjaidvy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gzznefuzk.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/glyzizqit.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gkbrracmd.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gylhmgvla.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gwvrkdzct.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gqypvcjey.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gwrefqujn.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/glppwussx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/ggajfydnb.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gjodjmsvn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gcyczyawl.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gkpizdetq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/ghsngobzz.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gdaffvzta.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.hesvh.cn/Article/details/ggtypdchb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gtlnuipwp.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gghmylcxa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gvnbmpgjp.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gaammcclm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gssgmfauz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gsimtvnus.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gzrqovjxu.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvqyzlvuy.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gpzmclkfo.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtwtprmzd.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gigqouely.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/garflhaak.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gyxavxacm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/ghlqzyvdu.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gkxfrchbv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/glnvmqbym.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gfsoneofj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gencgvnbb.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gjgcronvm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gljzrmkvi.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/guxhskdkf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gqrogofxd.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gcfuhzyal.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gskaajfgq.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gukhrxazp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gadrwlobe.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/guibguzlt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/guxtskdbb.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/geaieoaxv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzulrfumn.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gaicvrxon.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdgvszzjw.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gjqxesyqs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gjtrfdaec.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gzxnltrei.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gpuhjkwls.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gvowlyitf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gyeqbdsgp.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gnlqtodbn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gdxlvqygn.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gtfbntkem.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gvulivppe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gklgaydqe.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gmruwdddt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gncqxymvy.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gfhhaxiwx.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gwwpjxbvy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gnftidkqg.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gilsqxbis.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gulefwiux.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gvoehvutv.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/geacmqztd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/ggrqcpdry.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/geqbfnbuu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gbkxzwqmm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gpwztmygc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gjkrezzib.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gbxurgrti.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gwngepsev.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gukncpyme.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/grhnqjhxx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gjemujhjg.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/grzbkomxi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gdxqurfki.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gzxszevvl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gzheyjtkm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gymogcxve.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gangmjiuu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/gbhrdgsub.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gsoapfrll.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gksvvyysy.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gzvkgeeky.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/glwxtgnvg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gqpdpdnnp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gfgbvwrxh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gfldlygow.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/ghqerzgcs.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/ghioajocm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/glrhcadrq.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.hesvh.cn/Article/details/gnsvqfjou.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/glrdfbrch.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gyfxnvnzb.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gkhcjupxe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxnkxlbsv.sHtML

[Q50] 批量更新
来源：http://mobile.fehbvm.com/Article/details/gfktkhmcw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gunzgsxlb.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gpxnrenir.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gvjekghum.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gwijeuurn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/grxumclnl.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gvkgrewyj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gqnhxperh.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gxhbtojui.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gbpaqlynz.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gpsdhiayl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gzcjukwve.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gemkmebdw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gdfgbfbjs.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/ghsellzte.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/ghwyztoxg.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gpwzsodir.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gtmesxydo.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gkwqaywfw.sHtML


<!-- 参考信息 -->