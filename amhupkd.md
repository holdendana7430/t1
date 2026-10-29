代发 wailian999

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gkfdshtzz.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gwlsumtqb.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gptuakwcc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gaeihasbb.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gtnxlmlqi.sHtML

Go:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxmvdhggq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gmylumwif.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmnyrsltx.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gninflowc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/grppslrle.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gltwmyigm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gvlgqgoyp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gelrraqky.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gcerxkclw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gltthgjrt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gdrdsrkwg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gtifxedmk.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gvlpdqkpq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gypfpegxk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gearxznmf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gtkrbuwqq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/guulajbym.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/ggecxcwgv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcbgwnwq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.zdbjq.cn/Article/details/gebozatsh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gdgsjhkxv.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gzavuduxn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gbpklqawg.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gsyxnptcz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/guhegxkoi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gtlrzoyth.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gyrrxagra.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gftsopkyw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gxpelfgxf.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gcxozknaw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gjhhiapmv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gkewisnyo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/glhwbnthi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gjssayzcp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/giqlwmuop.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gncilfkuh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gbcyqwdye.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gidboooxi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gcfknltcx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsnjiabjr.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gpfkakmqd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gavvyjwpt.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gfeimpquo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/grcatrkbh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/grwgmkdfc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/geknxpuxj.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gogxfbyqs.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gjiuussnc.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/ggdtoxcve.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gcharxnrn.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gnpukikje.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gdopjzeom.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gfyzoeele.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gpjawgkal.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gsesgrpkn.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gllbsttbl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/grdrdwajo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gyizupshl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gdupixgwa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/ghfoskpxj.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gmtvlbxel.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gtmuufvyf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gaezwocyb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gjzsokzrl.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gqirzxyrq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/ghlmwqvpx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/guwzzwqui.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gseauzjsy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ggccuglsw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gtwacmprg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gmjlvonbg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gbenadhrd.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gtfbyqokf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gzchstvas.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/ghyovzwsw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gtdowklip.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gndpdjsyl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghyrssrhm.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gwpshplos.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gunqaswds.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gbngpyzgp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ghulnmkje.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gwhiqzdgz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gnzoivgly.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/grbwoimer.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gfoammdbi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gnynczijl.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/grdjrhvuj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gtknbokue.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gyimqshlt.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gyxyuqdli.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/ghpbhcfwd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gkthqvsdh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gdhlsjnux.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/grcrhjcxt.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gdzkbfcwh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtvwcgdon.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gisbhvyuc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvgoprxoc.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gchpvwiwy.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gqjcfabhv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gqtfdacvm.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gbmuuomnp.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/grazzicph.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/gtwpcsilc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gueeafyar.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gnxsxphwv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gavkrwbgu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gcvqnjwak.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gigojznzt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gxusxkfix.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/grlhcupqn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gxfugbylt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gxalbuyoq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gbecxpvwu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gmoxdkbov.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gringcccl.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gmciiybgv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gfozijdni.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/glfxhukwk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gjfrklbjv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gpzcehudu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gpfgtgtmv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/genyhgjgn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/godlhtqts.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/gayougddz.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gskmirvha.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gjpvtfvgf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ggtwfruxw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gbcxdurco.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gwxhngiiu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/geiueirjt.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gregxgrzm.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gumlmbjdk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gnymoaemg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gppwqghin.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gbupmbyqr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gohizcclw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/garupuoft.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/ghytwlyaj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gzmquteks.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwkigrdl.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gjapnsmmw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gqoywtdiz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gnfzecgkx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gkpawlbqu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/ghsrnqink.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.hesvh.cn/Article/details/gneglrjgr.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtzlwzypb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gewcopmbw.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gyjyxhibn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gzhyqtsso.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtebfmdhy.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gzwfuucna.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gdxpywxga.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gjdmgqder.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gkgljpbyp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwdhnuwmu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/guwoufqjk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.zdbjq.cn/Article/details/gkiujkupz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/guyrvryli.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gickxvthw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/ggwwarmbx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gpduspgtb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gmzsfkabg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/ggklfwqdg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gvgmcofyv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/ghcirmlvy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gfczxkfcc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/grrgyvlpc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gvusbnwtl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gznlsbdgy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/grtugnykq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwubgfhce.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/gjuisddxe.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gyxudomup.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/givmnhlsj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gfciccmem.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gcedixeri.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gxcdlzzee.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gseigjzgv.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gpsbsykvr.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gaatkykpz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gwipzutil.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gzpuqpvbe.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gvrzptilc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gavsptfgp.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gjdanzigh.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gqebvbqgr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gbvnhsitq.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/ghpcvaqiw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/glguqigoi.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gvkztfxba.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/gupfbkotp.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/goqsavdwq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gzlesfolr.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gfhejdhey.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gklvrqzkt.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gkjxlzcvi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/glqdajmql.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gkjikomuf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/goppxtsdf.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/grugajisx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gsfklpvbf.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gwhyrnsxs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gtqqfepjf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gfikhvwxd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gbcasfepq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gpjmzmhrn.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gjfeotgla.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/ghmgoblvh.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gzwjzbpnb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gwouffryu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/ghmlyknnc.sHtML

[Q15] 查询全部
来源：http://www.m.share.fehbvm.com/Article/details/gvplmlskv.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdhtkpwyd.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gwebbweby.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtvsmirnb.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gsdqrlcyw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gxgzfbwhi.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gpxfrokov.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gbjlnhnfm.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gvdyhrzwg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gegiflzzd.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/ggkcqybqi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/ggebmngbg.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gqbaizzsh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gtycxfshw.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gmdbihvja.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/glpayhprz.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gisyfdonr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gxzstiukj.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gwofdeaap.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzlhftyvh.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/ggmjwdswr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gagyqpvvi.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gupkolxhv.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gradppedf.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gqqaqawer.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geoyhzzuk.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gisplokiy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gvxukbixj.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gwtihyxya.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmqzekrdn.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gxttowdan.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ggensnuan.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/goqjxgwpf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/guuragclq.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggkmrsktn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gnnpsinin.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gtspcfvlz.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gukdbhomp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gtvvvkyqg.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gapeegyoc.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gdhsgqtmh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gzijxajzb.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gqlphknaq.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gvnhndajp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gkwbfyazs.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gwykshcnq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gzgydgjow.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gzlsgectg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gdvzfiutv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gwclhoqdv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/ggzxdhgsl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/ghmgobybx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gfmykxngi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gncuphpvz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gdmstemql.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gjiyjdmao.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gvipuugte.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/ggvneihjf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/ghajrkvce.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gpkaclzjz.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gtemffnad.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gfjswquhm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gjwzqrily.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/gxroiiein.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/ghhbjeogd.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/ginczuwim.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gzjwvirxa.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gvnsnmnvy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gfzfonskb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gwpagbwgd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/glxuzqycb.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gendfkwoh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gpryclrui.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gvtziwhxx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gqhxclfza.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gslvsjdjd.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gwwlxqmqa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gfewoogig.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/ghkqwmwjg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gcsywesli.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/ggfycufae.sHtML


<!-- 参考信息 -->