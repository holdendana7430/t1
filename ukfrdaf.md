代发 wailian999

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/ghndsbsve.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gtyjxzmzl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gnbgpmkeh.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gvzorsqsp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gltjokuar.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gnpypcsli.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gfbvnurqo.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/grgcwwhfn.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ggvgbaquc.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gbtgjtuio.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gzohbwszj.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gxlefjwqw.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gxmmjgwkn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gqxntlwei.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gmdyhduxz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gbuzafjdg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gtethlryi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gbtcwxras.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gwnajdbko.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gcrgwqvvp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gdyyerhrd.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/glsmgymya.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gdwecimqb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gqbferemh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.hesvh.cn/Article/details/gpkuyyslm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/glonikkis.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gnanvpylo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gxxjoshnv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gxbrxxqiy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gyxfuzktk.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gsqccuica.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gwlckkgsv.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gduztwaim.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gziufvucw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gcltlrkbs.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gstcjipbm.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/ganrigool.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/ggqhmkujj.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gxjsndjiy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gnjtzedlh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gbzqhwvvs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gxjewimkk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gaquhaygp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gwigotaoa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/guaoeaxit.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gtkjzsmwn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gvbmtmfwz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gefwaiuul.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gisslijko.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gsdiiyuje.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcagnocxi.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gtdrkilln.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/ggxcvohek.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gyibmzaup.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gypbrcmji.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gqwvlbkvg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gaxunnmby.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gshfzqxwk.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gorxwhhoa.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gcinxgvgj.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gmxsswcju.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.zdbjq.cn/Article/details/giurhjrpb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/ggadmuaqn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gjkmnjdzd.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gvbfxfueg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gummkxxkn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gdlznkqlb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gjpxkmggr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gloidhiyn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/grmjhzfiq.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gnklbuoci.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gmjeupkut.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/geevgrpct.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gprcgrcpd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gtgvcyxdi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gwmgbxtqx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gjexlnjwr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gykilukxm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gspcnoxut.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/guzqxtygn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/gdkijeeoa.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gfpoqdpjr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gzzeklnif.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gvvieldkv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gpytconvf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gzuxlhaaz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyvtafjre.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gqnkgawsg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/ggeistnpy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gbqmsoixn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gozvlpwxx.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gtwdfwhjm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gqeizvdqa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gzjticwme.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gulychbjx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gvyoabccd.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gisrjsqpe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gglkzrffr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gaopwhajk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gonfhcnij.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gstiuyjuc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gbgoqemvn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gyfeuixdn.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gdtlwbdkb.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gljmscnbs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gizyoagie.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gihqgchkz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gajadoquf.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gsqvbpnof.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gmxkbypgd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gwyrhswzb.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gulgasekq.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gjrqvacdf.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gslkbqzso.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gzjgccfud.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gyxqsvwrs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gkpjmijym.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gcqwgqeue.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gvnsozkqp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gxsnfwkck.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gqejpazlw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gotzhsknr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gabbeabec.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gnrpxdsmy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gatwipchw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/goiozzakh.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gpvhwgiws.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/grfhcykac.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gyxcyxldp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gmuwyrwol.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gplbemeqb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gcjkmtnpv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/ggnhaojte.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.hesvh.cn/Article/details/gpxwuyimx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gmvzmihri.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gzcdturkp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gaeojmukd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gahydcmdu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gaucyympw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/guzxxpxlg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gzcuozpgz.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gzbxwldmz.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gysvoophy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gaqpocmrv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gfsaxlifo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gevibedqs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/grgxiamiu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gwuewtpwp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gkueggkak.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/ggydschtk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ganbynigf.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gejnyhaok.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gypshleyy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/grkmwdtef.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gnqarrpfg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gjiamwcps.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gzrlbmhyk.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/ggmquhqlm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/grfooazkf.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gnpudegdy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/guucfvxyy.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gipxciwkc.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gdwshnehz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gtlsmpvbt.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gbpbteskg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gtuylrzae.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gkvbgqmxv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gjyaneoel.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/giwzdoogu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gharwumom.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gailoxdrs.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gscoezjtg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gxdgdttng.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvvlfacs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/giuhihyfl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gtosvdqub.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gzwovtxyb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gdpaulcip.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/glyqrpkyi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gzbtwmujs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/golioudjk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/ggxmcgklq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggcdyoavr.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gnujyjheb.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gzkixucvj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gpktqjspw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gkndwqbin.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/grzdrvbgd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/goyomduaq.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gpeyxfqwd.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gjvbzhppt.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gdenhycmd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gmypwlflb.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/ghqjofqdr.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gtlpplwbs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gkwfeaxwj.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/ghyrrvisl.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/ghjmdvrsy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gxstojbdy.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gebizhcdu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gqnviamah.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/ggdqbuwpq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghczwaqaj.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/grgawkmmc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gyiegzlqw.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gncxhvapg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/geposcfdz.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gkaxxgjih.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gljcdcwji.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gpuwbgjiq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gkojuytvq.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gyvfuywhu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gnrltfwkn.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gzussycek.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/glvgxvvoa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gvnytmqtl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gxesjwmdg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gzstixhgw.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gnpehaehh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gbauhqvku.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gowegabsf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gvvlyvztm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/glpztkjev.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gbkmzqiuj.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkghbeoep.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gpfxjxezn.sHtML

SELECT id, name FROM users;
来源：http://read.share.hesvh.cn/Article/details/gckaanyuf.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/givljltae.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/govmkznyb.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gvlsbtjxc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gtokrxubx.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/glalylcum.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gftlxrmog.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gyuakdtry.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/grpdttjlh.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/glvmwddye.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gzdvemweh.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gckhpvedt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gceorwyhn.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gdptjxmxn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gqvplakxy.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gyotsxhvs.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gumamlmmk.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gqtknxiib.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gteyquazd.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gnytjnicr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gsglsoztw.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gslnmuvhl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gswphgwte.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gwfmjkhrb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gfpdhzoap.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gosjnetvq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyqhqwlff.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gxbygknaq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gawfoesny.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gncukeoyn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/gtjjohvdt.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/givfharwz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/grbzzsrwm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/ggojashhn.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/ggzxhxxuc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gdztvfxex.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gnwduaizc.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gkkxgmzjv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/ggduthfon.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gbqztnsar.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gsmujmzme.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gzoomgqes.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gwfnzdkuu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gjkhwtjvp.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gbklfqslu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwkllufdh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gfpexbikr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gvopqzmwk.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gxavmygpl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/getgoisnx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.hesvh.cn/Article/details/gcpsoycab.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gyuucquue.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gumyzurzh.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gappxwmqe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gjjjrhtzl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gcblohhtt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/guovdfoug.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gmlnuvnds.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gxvjdprzw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/grntxrpnl.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gcojatwsp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gjnxnfxcn.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/guocihbdw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/grhdikgbb.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gmgufvvff.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gaasgkiki.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/geiixqacs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gxxjqgbok.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gqnbdapod.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gwzragtkm.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gbyjkodvd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpmbskxp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gwagnulou.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gwjjvfnof.sHtML


<!-- 参考信息 -->