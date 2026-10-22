代发 wailian999

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ysmzrpef.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ktjfafil.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wkbpyxps.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tfsxwkgh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ycvovtoa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2irxitfus.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bccyuhow.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hawgqgrq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2jilsybts.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2unqbraja.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2sjlsdbxc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qwauklix.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2swbmovpc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hvdppcha.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ldvqfofj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xgdprgfo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ifayheys.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bwcguubi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkwkaixg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2pzmhljof.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2xyoxilgz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cypkziof.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2efbvujuu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2yynaopis.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2sbdbmibd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lsmtzzwr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ussgdgib.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dvwmmezu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ypaquwno.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2aasteymx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rmhdvptm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2aqashawd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xofgxctz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wggvbcjg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uappjozr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2frsjkkhu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hgvbfxyo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2wdatqssc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xiwoovus.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bvrpgjzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tibrewsf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mbydlone.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvrobovj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wqgicmla.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2hqawflit.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hsabhczd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2erjtyjhp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nycqglgl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zkcwijjs.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2islsovso.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2sftvhawy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2uzytksca.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nrbjyzfd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ekfftozb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hggsyrnk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ngjvzqlp.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jwdigpov.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bpvwklfs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2tpgdofwd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hrxtzibj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gxoqpbex.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2obtpymmn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zzaqcrnd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2oymuxjkx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2wsahnpps.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2musvfvwy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rrwgjxix.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jwyscpuv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jfpjalgh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgygnqff.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2odmkgsie.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2xxosgbuf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2sahrslps.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xazdojxo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hadpggmg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uvbdavxh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2tnsabakl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2miytoyul.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2rswndfus.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2nyvyptdm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2psmbgfgt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cvkeimle.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fhcnromi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tdxzuvqt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2whpaxbxf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vkmdguzo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2qoikbwrc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lofsytje.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2fhdnfvoj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qufhiyvd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2awgvdfth.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qkgszedp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zvuucspi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2dnhlroic.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2khsycvoz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2aottougt.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2pjuizbpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrctoson.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbreskxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubknzrli.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cfscbvpz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2fyveopwu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mdausqwc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lfmcdbfj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ivvqcwws.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tkgbwxjh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2eemrzkwd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2slqvmgxg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2lhjrtyvi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dxedxwch.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2deznsrju.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tjirrtuk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lpovgayz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2vgdpzgsu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hyucluis.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bwsgbxnj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iitcrwyu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2khqlnoxw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ivdxcqby.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2iknrotkp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bevrbrmk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mxlwmadx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wbyroxka.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2dougvbwx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2waceshwd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2moitflly.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lrepitih.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jiipjydo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2qocukguo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ksdftmis.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ttpezmpd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bgcaxkhy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tyncrbkk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2rdbyjdhi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2lolwacvz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2skjennul.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uaonoyxs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2igiikzqa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2cdjwpuyh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2fbpmdrlb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2assrzrgw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ynoamaxq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cpffwyzj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2fiutibvz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ccfnotzh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uybzbeqv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rwhkvwaq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvildbds.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2xoqqeyam.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwbshjri.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwwqacuy.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ojxswpre.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dbetptho.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2caqpjecu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jjseqhfh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fbvwgwqp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lvxzdkss.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2drfyipto.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2agrvdxoi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2laowsbyf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2fgniqjyy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2dwsmxfyi.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2lqtojplr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2heqfnvrf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vctwjwkt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vqemhvvu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2irswyiyb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kpdxlgkk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wibxogug.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rikvvkir.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2myzrzubn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2husrjbzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzmfvznb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2kxsjdwql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftmcfkba.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2coywinyx.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2uvlggqmd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2fabnblwy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2nrgaajfg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2uksadncq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qlnxtnoi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ujtcvfwy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2xbhbcotg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2greecedv.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xiqcpmcj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qofgmuri.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2oqbmvuvr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2srnouuik.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2kptsiseh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qkkutvdd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zgrynjqx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2bovfiumd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2gplriwsd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2illrdtze.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mvvhftdp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wpvnefdq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ulhlowro.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ofjcmypr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2msllfvgn.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2sassinqw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jtluwcwd.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2iufrsswn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nswtjogd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2gprssatw.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2asgxvajb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ytbwhskt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2hwxwheua.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2cnypcmkw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2wtemhxts.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2gglfipxc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2iyqjhcor.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pqnaalra.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2hyzsugij.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2uxkmsopu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2zdjknzcz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2riktbxla.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yresxwpt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hdhabker.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lbecgwxh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2zscjasws.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2msaxjawq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2zvvxbxby.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2arjcbsml.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2luarrukt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yzsopcbx.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hxmjdopt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aqzohvkx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2uzngrcvn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mnsonrrx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bmnvuvaq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2lrztweqn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2zzdpkbtt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ubtbxzoh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2blzlzbqz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bhwbhuck.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ypbjqxka.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2cxwojaez.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2iykjsccq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2esthlcpf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wwkgwogs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ubxswtee.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2hcnjgdkv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zeajxpgk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ipczlzif.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fjwjvubc.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2kynmurjc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pfkpkfpz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2isjevepl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pnwrwvyd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eevgtewt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pgtvgvgp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2omhapevg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2lmknkelq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2xdbcohtc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ytuuqpst.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2otsehrfn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ghghzhfh.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2xfyeadsl.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hcfnhsky.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fpzgfpfl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ynbwbqor.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jvkzqnen.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2growpmet.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2sfoummel.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2rabtqbtr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rsjdkcqx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gyumntop.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ymewrhsa.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ysqixwdh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2xieludvl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2edkibnwq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2uhesfwou.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2gsqkejrq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kmexsaqm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2prtwevvy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uzefpvsl.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2pnregawj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dhythden.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2npsdxfkr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2bfdnbduq.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2pwpvlffl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kzxcesty.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2avvsecml.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2chgvkjbp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2vpcvkjnv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2birgozrz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2idfxbaiu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2hrwlmfzx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vhifpyyz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2vmtkmwfe.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wvnffshz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ixwtqnkb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fkwevzdo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2asybxtdc.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qdencvkw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mxdwynmj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2cufnnpzf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2klbxpktr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2lwewgfuk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yefgomds.html


<!-- 参考信息 -->