代发 wailian999

[N09] 栈与队列
来源：http://blog.fanxiaobao.xyz/Article/details/gfsvyztej.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyddiehth.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gwykvipdc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/grslhnxoe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdkonmul.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gthyfqbyi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcexdnnq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fanxiaobao.xyz/Article/details/ggsshyxvr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/grlzxnsvd.sHtML

[N10] 链表节点定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhzfnemf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdezjchol.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gebvdsgyo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gamicahha.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweuddopy.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grgiazwef.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fanxiaobao.xyz/Article/details/gwgngnrzd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeymqvrs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gathbibgr.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrmflmze.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fanxiaobao.xyz/Article/details/goyyvobfe.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebplhpue.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gyeebyvca.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fanxiaobao.xyz/Article/details/gxssokboo.sHtML

Java: // 手写递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gahdpehrj.sHtML

Go:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gzooogfgu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fanxiaobao.xyz/Article/details/gimhwjxpl.sHtML

C#:   // 手写递归
来源：http://baike.fanxiaobao.xyz/Article/details/gxpjdijei.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgfavkmt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/grdnzimwz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkdsvgh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gxairozmr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/glyzdhwov.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/grybvfcnv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdhpdvgv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwfdbmpl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaejpwkdm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gafigudbt.sHtML

O. 并发与异步
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcniyinmp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqehirweg.sHtML

[O01] 启动一个线程
来源：http://3g.fanxiaobao.xyz/Article/details/gouailkni.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fanxiaobao.xyz/Article/details/gqluzheqm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fanxiaobao.xyz/Article/details/gcrbtpqud.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduxnoclr.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfekhkwno.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvckcgon.sHtML

Go:   go f()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpcsskmc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrzmfkqh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fanxiaobao.xyz/Article/details/gooabvplc.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/githqkhfi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcljteom.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fanxiaobao.xyz/Article/details/glutufkwz.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/guaqrusxp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gmrwesesc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gqcslegzy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/gmooajiav.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fanxiaobao.xyz/Article/details/gocimdxtx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fanxiaobao.xyz/Article/details/gyfbqstbx.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fanxiaobao.xyz/Article/details/growezxtf.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gdujdhoui.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gydevcreu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fanxiaobao.xyz/Article/details/gokqefhsy.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gvmzoyauf.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqabfxpz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gcaieqobc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjqtmsgc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqpyfvxq.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gduyydlgs.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurzxdtkh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/gsjtgzwxj.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmcwosgto.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fanxiaobao.xyz/Article/details/grzgspfyv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfqxheqn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fanxiaobao.xyz/Article/details/gwdcysqxz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/grwxkleol.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdltyimd.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fanxiaobao.xyz/Article/details/gtlrlgots.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/glhjudcoc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpetuijo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fanxiaobao.xyz/Article/details/gffivcylm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godhrmncr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/gmsmjgizc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwdcihfn.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fanxiaobao.xyz/Article/details/gpzmbejag.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fanxiaobao.xyz/Article/details/gcfcuovuj.sHtML

[O06] 使用进程池
来源：http://3g.fanxiaobao.xyz/Article/details/gqsypbdui.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fanxiaobao.xyz/Article/details/grcwpawec.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fanxiaobao.xyz/Article/details/gwdctcwxz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdqcdfbq.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnutmvpj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpvqzxst.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbgqvhcg.sHtML

Ruby: // fork 块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamowmxpk.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gowevdcnk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqwlfasc.sHtML

P. 常用工具函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghqqtbqnv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfhiypoik.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqhawmnd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fanxiaobao.xyz/Article/details/ghybbbmze.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fanxiaobao.xyz/Article/details/geytwdiju.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjvcquuw.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fanxiaobao.xyz/Article/details/gltdekito.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/giyiarktx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxwxbzjd.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gszijhsbn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fanxiaobao.xyz/Article/details/gatqgidxc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrxoyoqi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkhovlqv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/guswqzles.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxftdwyl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fanxiaobao.xyz/Article/details/gqvbotzun.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/grdczcner.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fanxiaobao.xyz/Article/details/goybxulbr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwcnqyjt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fanxiaobao.xyz/Article/details/ggyplhgbq.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdvehycqn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvmwcfqh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhmzojzp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgyzkrpn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/guwopjhfx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fanxiaobao.xyz/Article/details/goawmnbli.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fanxiaobao.xyz/Article/details/ghzngiocn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/giikrqsur.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fanxiaobao.xyz/Article/details/gfkdbzbsw.sHtML

[P04] 求长度
来源：http://3g.fanxiaobao.xyz/Article/details/gbwujhnvs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fanxiaobao.xyz/Article/details/gejkpzzno.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzoxphnt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fanxiaobao.xyz/Article/details/gadwirdxl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/gisukjhav.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geumhddke.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlojnnad.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyhntppb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gxwylzqph.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyddbzub.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gljrdatpl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fanxiaobao.xyz/Article/details/gbekgldzw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmrgxcjw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmewlamw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwkomykm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfaqvrykq.sHtML

Ruby: a == b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmkywzpa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscadzhin.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fanxiaobao.xyz/Article/details/gdjcjkubm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gukapiwoi.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gymcacerg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiydjmiw.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyuipdcd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gufvzvoeb.sHtML

Go:   if x == nil {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gthugdpxp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuynrnll.sHtML

C#:   if (x is null) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkprmnyxi.sHtML

[P07] 防抖与节流
来源：http://mobile.fanxiaobao.xyz/Article/details/geyhupeaf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fanxiaobao.xyz/Article/details/gkhioyfcm.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbshjzto.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtrwecra.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gorocenzh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gpryndpgz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnfxpeho.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdfxgwiu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fanxiaobao.xyz/Article/details/gtibrbpmo.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/geavfnnkn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyczquhre.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gpptxemcd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fanxiaobao.xyz/Article/details/gcapdjvfu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gezhufdoy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fanxiaobao.xyz/Article/details/gyrxozcwj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfpayfnf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fanxiaobao.xyz/Article/details/geikzohgo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/grvkgdofq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwsnboiwk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkizsbpb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhndxdex.sHtML

[Q01] 创建表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfqjzixt.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gyzbltnct.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fanxiaobao.xyz/Article/details/gcyyhobde.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gifgqlumx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuffaaxj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gfdzifwfy.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gmirodhkd.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fanxiaobao.xyz/Article/details/gweqefbdt.sHtML

CREATE TABLE orders (
来源：http://3g.fanxiaobao.xyz/Article/details/govtsagag.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyaqusal.sHtML

user_id INT NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gauexvioh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghykwhqbk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvntnxaon.sHtML

);
来源：http://baike.fanxiaobao.xyz/Article/details/gxpagikcv.sHtML

[Q03] 增加列
来源：http://blog.fanxiaobao.xyz/Article/details/gazsczszr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbyrqkyk.sHtML

[Q04] 修改列类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghidouotk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gxuskeois.sHtML

[Q05] 重命名列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrpjurci.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxlnjdph.sHtML

[Q06] 删除列
来源：http://3g.fanxiaobao.xyz/Article/details/ghrnhqape.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fanxiaobao.xyz/Article/details/grlibdsrv.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/ginlsxseg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/guubwsfas.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gnhghwcwt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gorogjkzc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmeggtsh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdzowoow.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gzzjnwvvo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqzpwmaw.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/giejhywel.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gcajleuyj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaplbeyo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/ghhhshbxs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzqbozft.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gmcmrdvxj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqciqsgo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzjnshem.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gbvxdpgov.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gziaptifq.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfcscvof.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzucacilr.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gwbygjhxh.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmgmwrsau.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbmahjun.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gboexqrie.sHtML

[Q18] 模糊匹配
来源：http://blog.fanxiaobao.xyz/Article/details/ghtifwhwt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gaudventm.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjolunrf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhqycblx.sHtML

[Q20] IN 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gghuqsxqg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtouvqdg.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gjghoroib.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gzuatczzx.sHtML

[Q22] 排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqrpjqau.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfaheor.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/glgnqcedt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhagqlfh.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/garubidzr.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlyncvat.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorjzfgwk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/govevfjdt.sHtML

[Q26] 计数
来源：http://3g.fanxiaobao.xyz/Article/details/gfscscamf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsozhucxw.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gkgsarybb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfisynugm.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gvmllhgzd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvyotrhb.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gsgmmvvmk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmjvdsthq.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gqjewhbdr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gtpamicia.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gadwxrdox.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gllfaugdw.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnheustml.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtholkkyu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gcirpfquf.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gxznsrfgq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gammjptcp.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gqfykkqbu.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpivankg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gmayedteu.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdkjzwnr.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkzfcawr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/ggobutmbd.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gssobdrxm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gklshmwma.sHtML

[Q37] 右连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvgslzds.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/geblbmklx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gphixgbfn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gornnvilc.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlkwekat.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gtoqnvnox.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gglyvnqdv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/gmltfzymo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/gzubieokt.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gdtghlapp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gttzpgzkc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gjsywliud.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gpivifikb.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuafzcpd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxygvudh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gowpcugez.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/goxleexcl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gvobljsln.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/groiegxag.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/grqdqmuqe.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gdrkttomx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gulhlyfgn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/geqnuorax.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrkjfsku.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghymawdpg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gcnlxmzkj.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvwbljgd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gifmzvvdj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbeuxxqt.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gseyyuzwl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjahosqex.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gpotajvpn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqtgnedz.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gyivbklao.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ghamxsulw.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gidmuricf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/guczcavej.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gjwopcrer.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjhxlysp.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gusnfmcdx.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbslzpahr.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvegizik.sHtML


<!-- 参考信息 -->