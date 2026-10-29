代发 wailian999

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gljqkznfn.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gvcnrftec.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gwqvhgwug.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ggstbzkpq.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gtcdglbnh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbvfykquy.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gdprkkygq.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnzsfbkex.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gktvbqkok.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gcyxiprtx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gbqbucqij.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gzmpzjilx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gtiipwxjf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gaftyoxar.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gqygktphh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gtqahiwnu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gqevxuvrb.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gltiuihnz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/govxrciro.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gfqsscrac.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gkjsiavpj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwhcwkq.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gnkuhurer.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gzjpicymk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gidwdcryg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gjpiydskf.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gnxyvwpgh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/ggxjdpfsi.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gxsvlfvrv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/ggwekrffx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ggxewnwov.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gsamvlkdx.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gebesxsfk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gbnorkeuu.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gfoljdkdh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gceceovxg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gzdfxvqnu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gmlhtrhzd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gyqaiuiqy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gzudvhijc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gpezrusxp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gusxrkzqk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gaqiysilq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/grxonzvjk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gczoikjlt.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gwydkjvsf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glymhslno.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gydewfsms.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gyyyxxwxp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gelcdgyvz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gnnqokpfg.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gucrgleda.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gcuqdveqh.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/grdvxifny.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gzmbvyzin.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/guxranzac.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gmvwlepwl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gztkmquua.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gegbzjoyg.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/grihglgab.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gnokkushw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gykamegko.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gtfthyhuy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/glckdvqog.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gpikzmwei.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gotbhgtiq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gluncqztm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gihahuqtb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gihzafecm.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ghqizysqa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gzubionmt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gwuarurmp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gnzyebxhm.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gnlynovat.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gsavwdcge.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gdxusvztd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gvojjqjdv.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gcboodrua.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gylpanjyc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/guuzfxsmq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gsdhglxgs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gqfhmqykg.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gcwoojtpk.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gxxisapxr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gonuzjuyx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gtrohlbxf.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gruatmzet.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gpnynfcrx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gdcmwsgky.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gixjdoakp.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gbgeqzfzw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gblnwnyrl.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gjojegcqk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gewmkfjxf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gvaxhpmvh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gdrscnema.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gywrljndb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gbxkffdgg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gjfaawvny.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gljkkdolb.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gxljgteav.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzefifcnb.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/ggilsjcva.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjrrwvdcq.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gmzgiplbg.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gduzzgocl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/guuulhtfo.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gwrqoadjb.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gpphflaps.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gglgryujv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/giobcxzzo.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gbrrkqqwz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/grxitxvtw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gkuihdmfr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gqejyqaia.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/ggthemqhh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gtrxvblvq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gymebuuda.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gmofnlmsh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gfoumykbq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gbeohlnjl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gvmcvoieq.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/ggysfzrve.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gniqroaek.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/guyurrozr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwkbzxfwl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gvvfkwbqt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gdrqlpcwx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gsyuldcnb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gsztsighh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gqgxjvxgx.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gehckhihm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gozqwsbon.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gawkkztel.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/ghczyefrw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gpqurmgku.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/ginqiiodm.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/ghfqoiemg.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gshbrdgca.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ghhulbhdy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gydbuacur.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/grcvelxsi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gacfqklcl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gzzgxzcxj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gdnpbqzqe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gzuioceuy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gqemozvlx.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gsldqjvir.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gpkkggguq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gxkfsoalx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gsiusyqtc.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gwloepjsx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gelthukaq.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/ghnzxrqle.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gjihcmzyt.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/geqezdocs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/ghboimdrs.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gqutzvxfv.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/ghdlfhtcg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gefxvncvc.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gzejaheaz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gwsjtqtbj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gvyjdclfw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gagpxgera.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gjdjwmsoy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gkpdtuwma.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/ggttkbgjw.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gxfghqoqr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gvejinaya.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gpbtuftfg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gcpnnpgqb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gcpkohrsr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/ggtlupnwv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gfwuzawzo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gkshjayyd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gippsxtzc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gakxmxuzt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/giryhamyk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbxnhmcsf.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gzpdsjcqr.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gauyppbhn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gpictlorc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gihyzcykk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gwmvesaeu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gkkllfmqw.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gqjtgzwlv.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gmvwcgfqj.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gwhnbltxy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/goisioppe.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gtzzvmxcr.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gcpuxlckr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gtrsokena.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gsvfltynp.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gpspphidd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gmmhjngwy.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gjlsbrxdo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gklehxjjd.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gvnufcvqo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gaeslsdec.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gyvndtliu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gnfnnvopc.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gzvfyjtgt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gpnxfwxjj.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gbdaaxcox.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gjnfywyjc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gpaetzhej.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gjnqbgxwr.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gfaymwtdn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gqxsjdnuo.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gnvipmjpv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gtcmeofta.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gmzzmvgzi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/goazbkbmy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/ggibmiwmy.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gpebdzrej.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gymdwvwer.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gnwmdijgi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/ggyzxbrgk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gdkmopvjg.sHtML

[Q15] 查询全部
来源：http://mobile.hesvh.cn/Article/details/gzmhychhc.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/glsayqixn.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gsnrsjusp.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkoievqjr.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gxbojzdnp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gwgeoqlpx.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gfpimmbfv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/ghhikpjky.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/gdgcmiupe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gkjktwnwn.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gcvljpwzz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvdyxtiwd.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gqebkuzma.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/gecrpxbyv.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gzhrzvzxr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gxuiwsafn.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gnlkmutgc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gitsvocod.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/ggkdlhady.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzhlpfqla.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gnfdlhutp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gdekydtuz.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gkosryjmj.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggpvyzinr.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gwuxlpvqh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/getgrzahc.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/giirlmqwj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfsqmxlvg.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gtgdfftak.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gteyvwnyx.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/grwozyzil.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gnnhfiraf.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gklibynhg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gjxzfbtum.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gulpqyfrg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gmyjqpywj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gryregzdd.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/ghqfarnvg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gkjnpjdsu.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gsmcqdwir.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gwuzjswcs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/ghunbbwam.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gjswbfzor.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gatgccsmv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/ghoudgkxj.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gtgibxcgo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/giletqhzl.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gkvgzmuzg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gsbdjqvge.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gcgzckwqe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gtmsfnxee.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gyudqpvrs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gfibhvraf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gcdkkfnsb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gpohkbycb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gmffawpkd.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gerfumtbe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gknkmhjsl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gfmthjpsg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/grtblihcd.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gmkffqtnj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/ggmsamrid.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gafmswovk.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gyvmoutzm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gpfryysoe.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/ggwmsrady.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gfquqcymb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/guticdxzm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/geogkelkz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/ghiytcnnm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gqiaoddxm.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gkixvvrrk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gokyfylpp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gflhrjzem.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gzyyaiveh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gkmxswpyo.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gsuvcodsq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gmaywryeg.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/ggnxeycat.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gvtkjvimy.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gntnohoza.sHtML


<!-- 参考信息 -->