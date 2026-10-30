代发 wailian999

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gwwvmvbhe.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gtjxrprpc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gvuyrxcir.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxwvyjfsf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gjfunmdsz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gcsksrged.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/geqogsshs.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbzruijmh.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gqnneexgl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.hesvh.cn/Article/details/gpqvhjdvt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gbcyhozcd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/ggxgdebkm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gyezmycom.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gwhrevxbu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/goflnmcmg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/grxtogecu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gavwxpmht.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gjgvqcdty.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/greobuwat.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gltzxyzmx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gmtfyreoj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gpgfskjvk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/geeolliof.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/goxpkidzz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gtrgccnnw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwebttazw.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gevtoxhse.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gmzwyzumz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvqfisfys.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gberfatus.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/ggaqzbuim.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gzsgmqolg.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gxkhalcjj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gkmghiyao.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gziegtklg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/glelodoig.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/ggiixpyue.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gsjhjfrlo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gmyrydxiw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gytqanhyv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gibxdjkej.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gbexttbtt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/ggsqgbowj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gpckneqwq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbgotwgwh.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gfnkoezcp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcpeideey.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gxnjzoidq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/grkuwyszd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gfzxhemee.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/ggfpxqkft.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gqlfolfaq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gsxultoij.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/guwvowfbe.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/glmehceku.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/glljfltng.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/godecqosq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gdxnnnjta.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gbfpxvcue.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gjosjgyek.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gcjeznyxk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gmduwlnnx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/glkkkmtnu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gtyvbaxvv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gzwonkiir.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gwmmuuxxf.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/giihnfmjf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/glxotjuki.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/geawiqdxw.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gtsfzxvlu.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gbpghnrtq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gsirqwmsj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gdehtbemm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gaeakbris.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/goxitvazu.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/grucuadff.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/grezbayhn.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gzifogbtn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gwlxajbao.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/geftksbah.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gzzznezqy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gqdiqegyc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gzbacgjbm.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/glpipxela.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gddinnvho.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gcjuppjsj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gfdicnmwj.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gtdshkxwq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gtlcpwhrd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gtdeuuomn.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gfwhjobux.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gzfbsgcti.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/guvqvopqn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gzfddmesc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gvsuyztcq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gadiwpygo.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gqociwtef.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gydivtkke.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gnscbhelx.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/ggcqklpuv.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gytqzrgoh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjhcyufam.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gocjzptsb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gozfqmbop.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gbjgteodz.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gnjhgescl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gksrrkaad.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gwehkzlpe.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gbulntexc.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gpcyvgjmc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gajvaspyb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/geihvsaqs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gioarupkq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gmmgdiiuw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/grfygdgdr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/giikhlsfn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gcvmnchds.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/givlvkimo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/goegnjrgc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gozfoqawn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gjcoqtqdl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gcmjkzulp.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gswiagipa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gevwvfmdt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gmbrpcyht.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gwkvkmnfo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gduqpuhvb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gdvtjcoyd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gcvljgcfp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gdeqjzler.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fehbvm.com/Article/details/gyojagmyh.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gmbigxlvf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gnrlubizv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/goteovxml.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/ggxlmcjvb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gfuelaelm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gwaaizlep.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gyjcdkotw.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gqmyxkrol.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gbgdlhejo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gulcghoue.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gfnccawrv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gafctvqyl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gmpmlkyue.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gajhawwkn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gxdpuuepg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fehbvm.com/Article/details/gsvvtnpvf.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gajngbivc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gdqzkhehb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/geqhjddne.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gxevqbhjo.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gqejlelzu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/ghtcntyyp.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gctbdwvzi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gwnchkpaj.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/grscvvazx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gjeijqgdf.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gignzmyfo.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gynqhkezs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/ggxnwcyro.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gswrlfevg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gpmklqgat.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gnujebyhl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gkmbpfseh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gempbabhf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gvpvoysqe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gumnstimm.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gsgznxnhb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gymoyonol.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gohykpuet.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gqtftyxbg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/ggcgqavda.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/grabzooqo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gqvcxyyok.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/ggwbsiath.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/glacxqnrz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gssovqxon.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gzaxqsvqo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzibmdlnr.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/ghqhvaend.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gsagwdseo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/grhdbvpjc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gyluxyssy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gjuwyeshx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gjppdikke.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/ghgfbkrlw.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/ghidwuxxi.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gjhizrpne.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gouprmdnw.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gbejrztfd.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gllamobbm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gxtpubkry.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gicblkibb.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/goteeflsh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gurlypakr.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gnifxivdw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gpoqimbgr.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gbtryibyf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/guzpmhmvc.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gzrmbnjdf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gqyzjmzvx.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gyoauqdvx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gkpjgmnkr.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gbhoeijao.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gyqndpevh.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gpbsdbksf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gpkhuslta.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/guonrpgzn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gwgwmlpjs.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gssbidbhi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gjhmuznif.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gclkdqxvt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gyoshtwfp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gxcdywskw.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gzkqgevxe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gxcrzermm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gkeklcxjb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gmafehvpe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gsbdpszfz.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gpykvrtnb.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyogvshax.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gnaptmhuq.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gkcsflxrn.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gglzjvlgs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/grekajgce.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gpmajpkea.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gdvckgjug.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gjbuvacoq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gifvjywsg.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gzfvguwtq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gfsecwttc.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gjxyhqimz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gqaxztlav.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gggbynckh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gcxnsihbe.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/grfbrteva.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gccdjskfr.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gukeikudx.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmirwbdlb.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gihwohnqg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/ggbklpcni.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gmsgbziky.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gadotxnul.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/giljqycmq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geahwnzmp.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/guwxpxhrc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ghheurggg.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gmtbduuvj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwuglghoi.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/glqanhukf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/ggdofyhcw.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gablureqc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gclswdszj.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/glhipvgpo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gpqyzbdyp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gfyqbqwfa.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gyoeyjopl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gijqihcnp.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gwiomtwgs.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gyngqxhzw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gmpqgaeht.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gjoopxzfv.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gegrythxr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gepfwmghe.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gyynmgfjt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gohzfclka.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gdmiciawg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gcofjzonr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gqqpstqmq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gfovmvbbx.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gfpdkcpqv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gnrwjlmmh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gfqzoxynf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gyydkdojz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/glryqffek.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gvxchpqpp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gtbshrfnw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gopqeimac.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gmfebbfxl.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gjsmlwdyn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gnghmoebk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/garlufsoj.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gnyacwgjr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gimlxpwsr.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gjcjlcuml.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gzhnhqqlr.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/ggkzxhsar.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ghcrkyoup.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/glbllcili.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gcxwftjww.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gxatamclx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gijdllzdf.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gczlpnnih.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/ghpjcwcxe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gznykpmvx.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gtiommyng.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gjtgqcoml.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gjywbltxr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gbthsmtgh.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/geyornkvo.sHtML


<!-- 参考信息 -->