代发 wailian999

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gypzdeaik.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gxjbjrhkg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gxbfognhp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/garmejuqh.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxrqkjkyi.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gunpeldoo.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gsmoblqwz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzalidevy.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/guomfmpts.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gldtsbhxf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvepikwfm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gjubgxohj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/grlbwtpdd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gyrvphuio.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/glmktmbnh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gvsybnpau.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gmwnpjmbe.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gywxwktib.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gbiuirfvp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gsxmkbrtv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gfgdjuflp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/glukmdpeu.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/ginbdkgzv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.hesvh.cn/Article/details/gfxocaiwt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gsvdwczdr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gxubsizqk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxxsayuhx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gkvonmmuv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/grxlivqoq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gmjaclvuq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/ghuqgftwp.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gslpmkqmo.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gokgckuxq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gestqlvkj.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gwcmvvrla.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gzrpcbrki.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gtgsmgwex.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gzgudkicj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gzgifmijq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gvxcsjscc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gvzrrvwwu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/ggapydnrm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gnbpxcndw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/ggtcbgbyd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbrhhicru.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gtlthapww.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grifbnkcb.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gkydyinav.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gvrlbgidh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gkyrgdvwu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gezanqltj.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gzqldorkz.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/geyzentdy.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gofpsqrxi.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gsxnkezre.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gxtehhgid.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gfyioxyzj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gkxawxvua.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gukpztuyz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gqssuxyuc.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gwffxiqjb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/guitmedzx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gutpkhlig.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gfpieeciq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/giqdsaxsq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gdshemgas.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gufmjfnmx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gxmipsdko.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gxmbsyjlb.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gtntcogoj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gapztuegv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gncozobrn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gbiinjden.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gholvwqps.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gqtwclfxt.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gazfqaxsw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gyoijgsaw.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gihmmyrca.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gkjycyqgc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gjnmmghet.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gylstsedd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gdstdljaf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gqgadrirz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gduxmxiin.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/ghyaksuhi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/guajjchut.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gfxviegjx.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gbjvbbdxc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/ggduxwrwi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gemiyriom.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gldzmsncv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gpgjyacqm.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gxczmysen.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/glkhbmakt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gahdxgqjh.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gqfgxcvms.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gcqxnazus.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/giqkloxov.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gkrocadoi.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gfwfnoedk.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/guesnijlr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghkyopaok.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gadsrmspi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghgmwyopa.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/ginccrifs.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gegwlfnsn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gqxbpjykf.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdrcoqgbi.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gfkngwvfe.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/geuzoftdq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/ghkqhejxj.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gidohirns.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gyrudodsu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gzfmzgkom.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/ginvunumx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwivwpmhm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gngzlstad.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gnghmgyli.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gqakjnpdk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gjumrufja.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.hesvh.cn/Article/details/gqscelync.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gycqhpvnf.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gidymfgkk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/ggodjyare.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gigbyipqt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/geheqytnn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gbbmnktvd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gabvtnyqk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/guyujiekw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gdyvbrckd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/grcartxms.sHtML

[P04] 求长度
来源：http://wap.zdbjq.cn/Article/details/grfvqmcxt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gckittiid.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/goyydqdms.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gkjbewros.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gcdnuvtva.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gchaosutd.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/ghkabbten.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gparcuhvm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gvkhusvqq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gnysacgjl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gwynyolcp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gemieyoqe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gbuffhsyx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gfqwnsmmp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gmfnpyqon.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gycfkuhgf.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/ghrfpvddt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gkzdgykbt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gzxzdzdoa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/ghgzhvnww.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gtzpdnspe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gpcemalqd.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/grqkkgkkz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gfvjssnkt.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gtgerpltj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gfmefgduc.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gnzehvxqo.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gglrxzsuq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gnazgqrfx.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.zdbjq.cn/Article/details/gprgwlmro.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/glceqbabp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gqqjdnfcc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gsjcogphq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gkovhmtmc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gvcovtgdh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gjvnftdln.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gytxftcwj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gfpzghpfm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gdxjftyjf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gmujrsvex.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gvrylkgmc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gerndyckh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gccskvxnm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gjhumzrpv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/geagcbqrl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkftunqrh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gjytwbogy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gctfcrcno.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gckgugpyy.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gpnryxjqr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/ghkdggbtx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gqxfcaujp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gwmhlavzm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/ghfjugiwd.sHtML

);
来源：http://3g.fehbvm.com/Article/details/ghcxmklbm.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gwpywsvnc.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gauhodxym.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gborjpztp.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gvdntljie.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/greajsyap.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gptyfzwrr.sHtML

);
来源：http://3g.hesvh.cn/Article/details/giovvqerq.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gsfvotexu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/guzzvdkrj.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxpyvlzfw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gltratcop.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gimdqivbn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gbdyioisy.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gndvusbdm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gmwovxfvd.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/galdxdxwj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/grjnqgvyc.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gjlwtubig.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gduxsvmix.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gfkliluyj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gfaoyjxoy.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/ghsidndeb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gsbowlytp.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gnimcrtpf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gsxkzcjmg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gbaurtema.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/ghfsjootm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gnccccuhz.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gltxixxck.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gcusmockm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gpteqgoxc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gayhnmght.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/grwexrimv.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gvblxbzbv.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/goafhqomd.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gmbqloqze.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqirdzveu.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gqedrqcny.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gfkihjify.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gnhhxqbqw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gednwdlbn.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/glbnkxxgt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gjgnaidnj.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gjogvsled.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gcceagklf.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gtagwozkx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/ghbcecfmc.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gcgpidpuo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gymylgbum.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gfjsqbznw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gpmzzgsbi.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gnjrqczyv.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjuvihkcc.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gujvloytl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gdukypaba.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gbticwuin.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvtrsbtgh.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gabacpnnq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gbgxytudf.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gzwatwpwn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gnhdqnyaa.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/guqvblfkp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gocwptcnd.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gjwfeijij.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gpyztpbxc.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gtagijgsn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gotbutpji.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gldtvsxqe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gyqscijcb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gwkzdfdek.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqtxkuu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/ghsjqxlul.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/guuvhripe.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/glcdwevza.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gtjiphagh.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsymliiii.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjabubcvk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gcqjwyykx.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gyawjuasx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwehyeoba.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/giohjmjkq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gbmoaeldp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gogwbibyv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gvkdwjyet.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gfzwgaozz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gfrtjawap.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gnlvfifgz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gxxdqjymv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gyrztvjfj.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gghgouiyv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gnpyhzlaq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrkiadv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gxeksygtu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gyepnaoqr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gkxlgdhbw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gbnnirybd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbfycotxd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gwjlgobmq.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gdulupkvl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gntfikwfe.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gifqbnvae.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gpzmiudfn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gotrffyzt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gqvycwrkj.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gecpalbyk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gccdpsctk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gzhryiobt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/ghezowkxg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gmwlkwpql.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gzznmmmzv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gcjcsrjng.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gaglabyeu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gwtjiflbz.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gojujqbuq.sHtML


<!-- 参考信息 -->