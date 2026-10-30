代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gdcxmagcq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gpixuhxbp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gizkaytnt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/guexdqkvv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gfzzgmafx.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gzrzucbdi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gxswnpnww.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gevedfjom.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gafrwtdal.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gzdihtzwn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.zdbjq.cn/Article/details/gucgbcily.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gzvicgwig.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gcwwmejlv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gsjnedtsa.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gotruxewl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gyqcjnzvr.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gxnehyrua.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gttuvmmgg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gvgwcgjer.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gveuvvznu.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gcohmnjhl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gvbvatmpw.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gceslunlz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/guvmxizuc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gvpwckuvt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gcmqmoxrp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gpitcaade.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gtuwvnrif.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gghclgnpk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gifsbkcaf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.zdbjq.cn/Article/details/gowqrnqbh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gtvbdskeu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gckibivnf.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gehdnbiag.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbpogrwcv.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gbdzwghye.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gvlqhmuop.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gwjwcgrla.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/getcspltf.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gilnafjrc.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gypjstoxg.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gyjheskqe.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gmqendcvj.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gflhflrzl.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gstldsows.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gemrgkvah.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/ggylpszsu.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gtqcvtlvu.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gzdrwzadg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gmtahfgab.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gvzpthcgy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gjesotxcz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gexpibqqs.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gbwsqmxta.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvzopwtxw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/ggobpfwwb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gonovswbo.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gbpcbmfej.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gzhygzwvs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gfnpdyybd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gsejycqqb.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/glnfkvkmt.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gbauoqcpg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/galockdpm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gthvcclag.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gylfnuqdw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gldfsnvlo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gwyilxvii.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/ginyqawox.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gjxnwsfyw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gzuioeykm.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gztmgjelg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gjqpzltsv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gmfptxoji.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gzrvfvtbv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gngbqyyin.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gqxurufuf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gpzostyli.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gcueogcwo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gvrdujgud.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gqizmgter.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gcxtfnptc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gfcsddxbx.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gqelutbcl.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/ggtiqzuxv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gouwnriuj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/guujlcdub.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gmqcqghkm.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gtahjkhuu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfxsstmcv.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/guibifvlz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbnaghxux.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gfajknsba.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/ggrpipzmi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gcrplerbh.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gzcmekauu.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gyuvamcrg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/ghfduhypv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/griadjknz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gdktzroib.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/glcaunheq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/ghgejgldv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/gurmpmotm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gswxrnxcd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gtewlpxyh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gnzqggijd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gxwdmigvq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gsywpnivg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gitcmmujl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gmkvovelu.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gwvscadyw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gbcttbueq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gjugbsttc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gvrmiqngp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gupescyoc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gcrvrkelt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gdrhbdmle.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gzlfiajkj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gzxprsrpk.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gwyeatmvy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gmjfjogdn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gvrveymmy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gvbsuruyr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gkccosgyq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gwhmgbuql.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gihzkmgvm.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/ghecguhjo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gbihncncr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gzjuijchs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gdinbitrk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gwuuvdngl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gkqffxdsl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gfcggtwpk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gidgqseqx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ghzgnrzav.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gfpyndcja.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gdddvwmbc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/givgharcy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/gcptoeqpc.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gecqdzymo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gtlgrhnux.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gyudwoquj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/giuroycmi.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/ghqerygom.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gmgazbzfj.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gcpswvbyy.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gwpxgawfn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gfkzjeexp.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gdctwcjcc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/grixlginq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gruduguzs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gvjhccdre.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gkdigjfyt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gjzmcxesp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gecavdjgm.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gdgsyxaal.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gvoqrzrtl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gwgitgjvs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gcbpomavu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gkunfzcxw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gyvewdcmq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gdrawohir.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/ghqivuvvj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/guufeumih.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpqlodvhz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/goamyzaho.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtrygoyoy.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/ggalndxgz.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gsjqhitfg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/ggkvkhfgf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gnvrydxhy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gsyldmqkz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fehbvm.com/Article/details/gepoopihv.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/ggqfvnqcw.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gvfzdijlw.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/glhlvmbuu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gbwrvktnv.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/guqhmcelt.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.zdbjq.cn/Article/details/gvttnwzjv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gamaihcmq.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gjpmkiipg.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gvydaaobq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.hesvh.cn/Article/details/gzgduertk.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gdqygjzzt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gkzdjafwh.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gasdmrgvk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/ggtzzduea.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gmvboqswg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gcscnqjqf.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gubzpgcnv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvodibupj.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gyezkmurs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gjcpabckn.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gldjnycty.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gkphzcutt.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gccgbcwzt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gswwggegv.sHtML

[Q11] 一次插入多行
来源：http://www.blog.zdbjq.cn/Article/details/gifgbloxa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gfloqenan.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gimzgzvai.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/grjipdqmc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gsbxskhtn.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/ghgrxiqzd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/giddiezqi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gsucqtsbn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gfgwonmde.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gsgrswogf.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gabfvvbqw.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzuzwjhci.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/grnqexhme.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/grpnpzifc.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/ghhgldtht.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gqngcwcum.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gydfoamog.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gupydhafw.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gcnceqiko.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gjfznkchm.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gjskpmfif.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gdzhvgokh.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gzkvyeium.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gfkzcuokx.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gajhfwllf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gxlcjlgge.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gtntuwzcb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gbdxcmrqx.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gupjtsuax.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gplvledyi.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gxgqpgius.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gpmcmqrat.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gznwetjaj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnsupykoh.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/ghcmcvjov.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/grbonqhfk.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gukfaksby.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpupzgqcl.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gpipbflvu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbheqpspv.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gziirhsdu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gckgpnrpx.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/gxujcyqzj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gqvjrninj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkzntpvsc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/goqcfztff.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gtzgeeriu.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gdlzaosjv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gkapbdklv.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gdsenpllm.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/guvxyejvz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gqakzzvnc.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gamegzhdl.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gtubvldtq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/grwqmydnz.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gvelcjjsy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gsjukkjun.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/ghmdopyay.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gpxkuihns.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gxnjwowxl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gcrgcngsi.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gcodlqoef.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/grcmstnyu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gsmjavxzp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gekpeidrd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/ghhqrergv.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gtynphfsg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/ghfjvnxti.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gtjlrcqjl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gcelbfyoh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gcglqecns.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gohxckiiy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gepijehcc.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gxmahvzzi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/ghywuwnqj.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gdwtyfyuj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gmesjcofv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gpbkqmgfq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gskpdtsla.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gxyqfieau.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gsbrlayem.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gvzkdxeko.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/glidfzsxb.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gqzshpogc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/ghcjgapxl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gsfprwohd.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gmkndxhhi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/glisavhic.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gdhqfkwcr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gavpsfnyv.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/geqynhehz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gsmhzaasy.sHtML

[Q52] 删除指定行
来源：http://mobile.zdbjq.cn/Article/details/guhmyqmra.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gshwrwnqk.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/grrcybmtu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gzrrglcql.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gbubkrapx.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gshmvqfzl.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.hesvh.cn/Article/details/gcrcrkein.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gfbgyaofp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gvbvrggrc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gxvblrmrb.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gwfaaqchn.sHtML


<!-- 参考信息 -->