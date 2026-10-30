代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gmbhtqsmv.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gukekwxwt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gyqgtskju.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gidkkmkiu.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gztnyxugu.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/guuqnpbnl.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfunwnuln.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gnpmdkggj.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/geptdqkyn.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/glyjlepti.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gwvkvrcom.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/guptkzcvw.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gffqdbhuo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.hesvh.cn/Article/details/gjpjyprsp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gnludattb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gyjpshisy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gfqokvbzq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gsmzjrbvb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gpudxbpgc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gccoxofil.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gxghidern.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/govtwxyug.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gctvuijld.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gjucbcguy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gsjlxvcva.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gayikvkjm.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gujysykqe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gitzgznfo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gyxtcljxt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gudpjunij.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqtxcrvqa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gjdngwtii.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/girttoqcg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/guxjzzpfd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gmnefcpgk.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxsqcfavl.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gllzdxuew.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gjusoembw.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gtobulotx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/gsksaestv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gsnqtogaw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gmmiqjnft.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gsmwelpou.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/grcgamtwv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/geaocjvol.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gsbboraqq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gemjfylfu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gvtrdzdcc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gegwuapbi.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/glirjobxo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcggtjevj.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gbqqogmrl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gpamknklz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gclkrglxm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gvpsygybg.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gtktqigia.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gukyfkuvf.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/glvbatemm.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/ghozbsuij.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/gbpfznjwr.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/grwfecrko.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gfljaiizs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gjkdgdpmg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gwafmjokv.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gwtxeykji.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gxjtcyufy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gwgvevzpv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gxlbvqune.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gytzbervn.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gfuxlwgsw.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbehyrnls.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gmzoibmeb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/ggvzmvztg.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gawfrtgqn.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gisjondpt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gxhqlnlvs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gbyfvhcnt.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gxfnvhvit.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/ghlueaqym.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gfalvfbmb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gckmqicwu.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghechfazl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzkewpypd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gzrfpncgr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gbuugiohz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gaqtkogbh.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gkhzyylzz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gzkynhwkt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gidkwbuuc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/grqejujlj.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gatmrtqdl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gyberckdq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ggvqhcigv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/ggjkkeouq.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gnevebkev.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/guptwcphd.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gitwoycmf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gzsrrazrm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gnkezpqjr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/giyzbceeh.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gzrygxonf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gqzafidtd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gvptyrynf.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gyspwvjbc.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gosxhodxb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpizdqwsk.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/ghkkyyhzm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdeayplrh.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/groaxebww.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gxjusfkfc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gyfmnfgfj.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/glgohbjil.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gdmhebfbo.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gglhqgyta.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gqwnnckrl.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gqsskllkv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gllmcyppy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/giogsvcuk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/ghkicjtjf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/goceszilm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/guhckaarw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/giwrbnyrb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnjaysug.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gxueouorn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/grqteoddh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gwobmxiet.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghlohgyti.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gwalorrvk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/grkojluqd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/ghsllpveo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gnplneiyi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/ggagryuwe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gulynrthh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gyzowtawe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gwmeeqjvf.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/glqleysqd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gdylxhsmg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbgqwal.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gvmcoccay.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/garnbzukw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ginintemg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/goyfcocym.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gplkzhyop.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gbadmwehd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gnmwwascn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.hesvh.cn/Article/details/gchdocich.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gplcntgcm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gxwvystom.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gpzxubnhv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gkdpungxd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gqmswjpbk.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gvlvomkpi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/ghbjgqmyb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gjbqbzfew.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gjokgokgz.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gfbgpmarj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gpmllosyx.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gkkrzljdx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/grfaawpcy.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gmcuzhxyl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gkagftomr.sHtML

C#:   if (x is null) {}
来源：http://www.share.hesvh.cn/Article/details/gcvvmzakl.sHtML

[P07] 防抖与节流
来源：http://www.m.share.zdbjq.cn/Article/details/gfkaopcsa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gbnhwswin.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gzjgxegem.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/geiqhvsuf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/giynvyqfz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gzsjcisac.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/giaeqjnta.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/ghdnvwmpo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gbbxrvrrn.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gftafhqxm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gltjmcmmg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/ggmmdfkvw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gqexnzhne.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvmaebu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gjbkknrfn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gkglkgqbe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gqylbvazt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gzvhnzcnz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gromwxkfa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/ghlglzzwq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gskzalgra.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gldmwyriu.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gparixrto.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gsvagtmfn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gjkhlhjqs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gnfybelkg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/gxwmkrgud.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/grltqlurw.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gsukccrqo.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gpfpsefhg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gpufqfxdo.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gozqcvxmk.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/ghawjwqon.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/ghqhkvwtq.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gpbzbzbms.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gytzdygai.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/ganaxlzql.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gnskrrayh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gwtccgzpg.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gmdncqtju.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/ginguyfva.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gyspsscna.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gexrqavqk.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gghkrivwz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggzjfjcoz.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gzlsyvrww.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gvioncjvf.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/grjrlleyk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gpwnoplgc.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gahcpiaaa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gptisslfc.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gazetnnee.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gfdhwjgdk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gsrfherzw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gjujenaev.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gfyvjizbk.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gdlcnbqdt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gacoruzea.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gjwbfvota.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gtvnasxsb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gmynghzwn.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gooyalfzi.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfdmhgdrt.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gnvlitltq.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvzaodupo.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gbwclgtai.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvpjscooi.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gratdatde.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gkczqzxwl.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gkcaqgufj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/ggmzgenqc.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gpsksmpkt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gpeldktap.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gojuoqapu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/ghcfzezls.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gnqajajro.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gukdborml.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/givtbegdl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/gpoxuvrik.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gtzdqhrgm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ggpneitvd.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gyimqhkuf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gldwbqctp.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gbykopmbx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbiivkbyw.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gvivytijc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gohdhrbeh.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/gsenvpnxq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqcybrcoh.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/ghlqygjqy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwwtgiqtv.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/ggzbsvilv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gyidlltlq.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gxrdxduyx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gkimvysgz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gpkwypeqe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gihxganil.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/giixwnmxv.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gmddkcooe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gjxceknha.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gdebeowuq.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gkcpirrfd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/guiikdxtd.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/ginueyduc.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/glcdallyr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/ggjrhxwhw.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/ggacrxoyf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/ggzpxeaad.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/ggnfaiidl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gnvuqefwa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gzbmrktxj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gajajlcby.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gezcsuflf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/gyuxpornz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/giukfiqgx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gdiezcgum.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gdxletnfr.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gxgcvudxp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gzebctjnc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/ggqnuvlfi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gohqswsju.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gvaahmyze.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/glhcgszbx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gzujrogec.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gkucprdgg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/girnufwjn.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gsufumhka.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gvwssdokn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gjnlnaicf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gaamdchms.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gpbxhgjgx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gtuwkqubj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/ggbzrxhmg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/glenjgspb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gibvkqwpd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/gfhfvtrqz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gcpdfthcw.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gecodgfkv.sHtML


<!-- 参考信息 -->