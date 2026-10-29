代发 wailian999

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gcwbffqyt.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfguzjjfa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gdschsdwx.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/genkfkevo.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gvqqctctv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/glqoffctn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/glndhxjib.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grlejsdgy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gwbkgmofb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gidopopki.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gdyrhjszs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/ggwnjnbex.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/giqbyhhlv.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gvcqfjdrk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gkvcajbec.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gvyltqepj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gnjvnfrye.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gcdahvnfn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gcjvokubu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gmucserry.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gyycfarqe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gyhnwhqzb.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gfdpbkzsu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/giszgqpbd.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/ghzlgvsui.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gtagilsbj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gaiellpaf.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gpnonghll.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gzhqttwrg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.zdbjq.cn/Article/details/gbgvsznvi.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gdnuuwxsi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/goaorneif.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gpiyhdntr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gelaywbhk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gvwazfgoc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gfkseaycy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/guillkrnf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/ggdziadkw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gcewihugm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/grrhodexm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzssbawjy.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gszwxavkf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvtoersqj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gvkqwksou.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/ggrtxaald.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/glfroranq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gpobhimax.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gyiptogmv.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gckldgqmi.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/grdezgdrk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gvtelejwz.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/ghmkxejrv.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/ghwfsuzqy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gfikziwjo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/gvmxmxckg.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/ginkixqgk.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gkylqoith.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gbptunkup.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gptozlofv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gmtwhwyto.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gbkvzqfvw.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/glntfubhp.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxxspqnpd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gqjaxmxao.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gioauvxvy.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gekyhsegp.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gejzwsvjb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gqdfnrlbt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gyndpgnwh.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gvfuiptnl.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gwnmifyly.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gjejhirel.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gcxzaqrco.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/grjkuupyd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gxligfdol.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gypbcvcou.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/glkglmrzz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/ghpczyuji.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gjlnighzq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gpddxltjk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gpwvsogws.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gngxcjiyn.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gtcvbqena.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gahvafuto.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/ghxsjsdcw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gjfzoscxg.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gjbkgvudn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gzurlwwjh.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gonizvpms.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gpxxdtevf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gykuvbjio.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gjhmlogwx.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ghfoblrmb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gbcoypofq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gpmbppcdo.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gfxwnuoom.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/grnqzvqav.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gddrvhvlt.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gllqkbyef.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gexjanqzk.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gieoluihs.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gpjylhswe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/geihvxsyn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gyogrzkph.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gvlhykxms.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gqcnijirv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gnviaaron.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gxpipxxeb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gxukljmgo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gjrxtfdwk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/ggqxlvicb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gwxbbqdzl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gwpzfziav.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gskgubckr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gisgpleza.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/ggpaqqwqy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gdrakpgsn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gcbioomyj.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gpzrqvumf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/glnqsxcsq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/guahhssba.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gaascamiz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gthcrpaoi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsbzpuyf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gblfkqguc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gbhselmot.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gqgtmprdq.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gskkipwhf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gohswcrla.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gpxqrfzrz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/ghwzqjgtt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gkrfizplk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gbdjqbucz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gxihznhfb.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gwpkmyzxc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fehbvm.com/Article/details/ghqbglumh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gvdqfmxdc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gykapxcjl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gijhppjkt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gfoavywsz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gkgjirwcb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gkdodopqn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gnpfaruun.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gmsdkzqsz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gzmotcjep.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gcadsdvsp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gkewkadqp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/glqzovkis.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gzycazsew.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gydowmvku.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gkvpcjikf.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gzalicrdg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gafhdumju.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaafqsrpe.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/grqyhumux.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gezbwpvxz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gnuwruibi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gzztgyivg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/ghyftbgbf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gcuzcllpq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gnbwspzdo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/ghxuaprjv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gvlypgzia.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fehbvm.com/Article/details/ggkvhrtsc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/ghyycyvqx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gxdhoswvg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gokgvcfvp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gqoxbuaia.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gwwwbjtdj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gphvhijqv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gtrytccfe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/ghzqmvbxy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guzhbwodn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/ghotwcibf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjdcegikb.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gjwpaaszr.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/ggcknqtnb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gstgqiahn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gvqdjtdkt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gsizgqqmt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gifsxjqhp.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gjyetjejm.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gqphhhjdp.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gysckfxds.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gejvebybs.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gpyywwgpb.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gnzmpntrn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gxsphrsdd.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gkpysmpbo.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gzdjrrjip.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gxlchqmkk.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gdipkkwyx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gmrsykerd.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gouaemhwd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gezcaphfk.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gmdypizlr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gwpwszyvp.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/glhupwsey.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gvvhrarqe.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gpwntpmaa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gazwhousn.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gbszaacih.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gxencrnyb.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/grlgfcgok.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gsdhpelvz.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/ggascotym.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gojrlrind.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gijiwofno.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gsyrrygry.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gexhwifpy.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gzlczqtzp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gsqgwgqxv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gtrvfroff.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/ggerziyyc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gnlbsagme.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gemfnvwlh.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gaobvzktd.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gwkgkeqke.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gqbavikbv.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/goqwmkaou.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/grdvbavbr.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghqvkuokd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gzdhvegai.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gtswgeueb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gvectasck.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gfeikvlll.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gztxoqgti.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gumiuaizr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gmviauvpa.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxejgzkxf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gudrglxmh.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gybcmpvkb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gahkobrnn.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gswjlvtjz.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyolfanin.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gvvijdxyl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/glwmvxjlb.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gdbabddso.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gadmtykpm.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gwyqixkhl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmpwswakh.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gwljxxyvy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/grlvzensq.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/giqinbsgy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gwrtxxwfq.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gungilwrq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gwcjqaoic.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/ghibeahuc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gxfwjxhuw.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gusiynyqr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gqlwsdfgf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gfrtyoayr.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gfwynocon.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gclvralgy.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/ghnboukes.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gyyxcgszw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gxcasjtqv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gadrlqsxw.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gqwfqquwo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gvdtrvcof.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/geljfmuuz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gwxygoydk.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/grjlpnmos.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gjqsmovta.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gbkqesncp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/guywrqlkc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/goufhdrio.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gbjdlzfvf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gdmkcgrwn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gzzzznfws.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/goyucathz.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/glreytwuz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gihdrhjad.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/ghwpcodgs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gjobnfqbr.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/giocapruo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/glkspqbpa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gjwhxujgz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/geiysxvtb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gcarpnhdw.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/griahthjx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gkudbpueh.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gcqofqlda.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/grrphbmbk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gizawtlmn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gvqckrzkq.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gebsovwtv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gsduvzzac.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gidpwxqjg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gtyasapow.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gqxsdgrji.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/glaqsoihx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gxdwoawxz.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gdroscgbp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gndlfeesu.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gjjzdnnrf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/grlwmckul.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/ghjpohedp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gdboqjtkz.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gvohiupoc.sHtML


<!-- 参考信息 -->