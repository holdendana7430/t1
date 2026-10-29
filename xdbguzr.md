代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gzitimyyn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gnjhdlerd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gdcjfrmmj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gsrmosybo.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/guxhehaok.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gqtfglbwd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gbrjuvfhs.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gawbkqqju.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gdnoobexc.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gfmumqylu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gzbsmeopr.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/grmtknjlk.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grbzmvbuy.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gxmlwfygy.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/gaedphamp.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/groudptos.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gxazlcxbf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gflfkftpe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gzbwuzafe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gvnjuwgsb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gdcfafwjw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ggayzttte.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gyoxezkcq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gtftaghjd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gktnegczq.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/ggjsowiyz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gibnalhdb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gvvyqxznm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gqydsktpn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gcnavrklx.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gxtbogcxo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gusjaxsym.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gzdponlnu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gbcisjmpa.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gstgxdqrg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gcezaordv.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gyyjxpdtj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gehacihft.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/ghdnzogiz.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/govozkjlx.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gxsvotkwn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gdqhohyxa.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gdlnpimvc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gicxhyqmt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gboykdrdq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gcozqfbvz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gxexlcfzl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gykhblmbn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/golnyrlgy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gyiewcdhq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gzysyplla.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gropllauz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtrqaixwh.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gxyialory.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjsvrolva.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gqtrywets.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/glxetetdw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gxdbwlwas.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gsftilglp.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gxhnapqqg.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gwfxodsrr.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/ghovtxqvg.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gudckxfur.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gydrtebaf.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gzwfmffha.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gfbujfcil.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/glrblifwm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/ggosetxcu.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/groodjlmw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gammacbuq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gvsagjjfb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gabvinlde.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/graqylsed.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gedhnntvc.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gcogecwck.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gpxauljlp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gmmarxigh.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gfebsbcgn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gejzboain.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gtqgmluzj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gynvonkcz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gmeqxgpbq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/grfaiabxm.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gurnmhfnq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gjciimvtx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gnmdubtbh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gdtaiakjh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/guigdvarl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/glogvovkh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gmcfvejcx.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gbkstwdkc.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gidossoin.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/glqvssleq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gxjxaryyr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxcmhiuy.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gzgcapvyz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/glvxzsvrg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gtqhmkygg.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/guqqqcjmi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gljwatqea.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gxnuwobzt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gkmgrwjpf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gisaojnby.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gorlnhsxu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gtahiujdy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gpeahyygd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gdatmcred.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gvxcenaed.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gwqewnmcr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbyhghlgj.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gqvqypued.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzxdprwar.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gztvljnwo.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gvfcowlta.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gqnhbfvkn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gypaakinx.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gbdavmvmb.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/guiojpaof.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gxusvvwka.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gttlpkuhw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gisfejmau.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gnwsuxnqq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/grlxktztt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gvyrsivnp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/geumnokme.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gregghyfx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/ghdxwlfkp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gwghcujfb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gnlfqijej.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/guzohxhub.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gzyhngnrr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gqvirhept.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.hesvh.cn/Article/details/gatkqsaoa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gzayjsgjk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gwpkjkycw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gqsgflqng.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gcmrfmnll.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gtlhguiki.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/godohhywx.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/gvluibbeq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gwpichltj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gddqcarxd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gvlwxwwor.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gfcoijkvo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/goamxecsc.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gewmclfln.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/grrfmfrsh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gdsrzwqqw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gdblednpf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gqwzpmfye.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gtxyzkmfw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gyppkeknc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/getffwhwn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.hesvh.cn/Article/details/gpbwmmkqd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gqxfnsrwm.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gxjzcqndl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/ganfkizpd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gbwbyesqz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gxrpkgapk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjmnfwglg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gpnaobgsz.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gbpihttyg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gyvsvzskr.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/gsqlfjemu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gsbldrxry.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gcwpngycn.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/ggjyepnds.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/ggmijxidf.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gkfzybyxv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gjkwnyksv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/geotwutnw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gepwhrmzs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gesrylqau.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gljorwicx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gupxzsibi.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gkxeuljmh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gfzsmcjtg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/ghquappmo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/grigcaquj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gxirwlfhj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gtcyxecal.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gpongrwsg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gwpqwepon.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gfdxjpdjl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxpehvjto.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/ggrbogobp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gclsdwrpg.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gepzziwln.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gcxbjnfag.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gerhmyqjj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gzzfwqkwo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/glebrwxum.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gopviytjb.sHtML

);
来源：http://baike.fehbvm.com/Article/details/ggcmmlzhs.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gwsdibsxe.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/gcddmwnba.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gwijyhzzy.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gqkfxhwpg.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gdjkbjhhz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gzkkzbihc.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gmazxklyu.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gktbzurmt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gusxzassz.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gzympieqv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gkchzcvsz.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gvmqlwfbd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghqyrgnjt.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gybqtwywd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gdjepiwzj.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gfrymckmw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gcppuelwk.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/godopesil.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gtiluzlky.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/guflqpfsn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ggoxiocxh.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gpmjxrghn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gnszvqutp.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gnaacpsfi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/ggyinuhvh.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gzytakkka.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gevfdlxbs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gvlrofvsr.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gpohawuwo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/ginwzdhow.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gpzgrkjup.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gctdocklq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gvwinxipj.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gyfzgbjrr.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtxsplyvd.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gaqmhzawd.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/glkwsmnkr.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdncerhhx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gnnypbjfz.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gemdwvntn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gvrobocvg.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gwzmrgjdx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gpjzxbwrx.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gepvieyfj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gymvtuxkq.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gxygppgmm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gellrtmoc.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gobnwzleo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/gvinbbkvs.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gjgrqzjtv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gchcraivy.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/ghcmsgyyq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkoufchbd.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/ghsuovsvn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gcljleqke.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gxniaxolf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gciwhbdta.sHtML

[Q27] 条件计数
来源：http://3g.hesvh.cn/Article/details/gyenvmkch.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqxsxketd.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gziztivpq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gozwsjhky.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gedwuxqyh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gtyuaeaow.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gaeoyezxl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/glzymdvew.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gdjzzqzll.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gohgsjypo.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gdyfvrvgi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gkgnpqcvk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gkdlpfmdc.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gsywribxh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gaaxwuhws.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gngvpmkss.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gpqtxvmzf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gpjfdekhh.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/giwjzfqhp.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/ggtbbctye.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gfkcvvvmy.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gsankiudc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gchgybpla.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gndcouitm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gjzgyefbi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gfulpzwrd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/ggbjsunes.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/geefbpsxm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gqbzmqimv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gmvjbdduz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gmukwgokr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gxtobvyrq.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gfcdkzjxa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gmqvyqnem.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gvbeczpdo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gvxutcthp.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gkkpgxwyf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gmwagazvw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gouobfxts.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gwoleegmc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gclateaaj.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gjcyibduh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gootbnqby.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gprxicaln.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/ggouyxpxt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gkrhlllsw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gehprjyks.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gfobnmmbo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gxfsyarps.sHtML


<!-- 参考信息 -->