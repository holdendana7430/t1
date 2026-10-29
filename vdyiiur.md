代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gqdcovxzx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gcpodnxkh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gwsodjomp.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gijaafsav.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gzbpyijmr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/guckjvcut.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gytzwqfbn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gnxwfppyx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gvhfwlohg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/glhgeqhac.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gmeusmznj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gndxmvnhk.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/gzolzruyt.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/ganwxvson.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gjhzwsddb.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gtcgfofsr.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gozvwjrnk.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gghhmfcbf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ggltdlvme.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gkikqryxf.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gwuwedhpt.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gwdioysfn.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gkfytgsdm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gmafgscza.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gjlfbkbcq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/godsciiga.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gdutqgrkz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gojltbbxf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gnrkesufe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/glqbscysi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gxhfidyix.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gjpasmmka.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gwdnpeccg.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gmydhawvt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/grygthind.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gzqjbewww.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gjugtcynn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gthprcgrp.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gazxiqivh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/ghpidzmoi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gbcafzbpi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gplstkowl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gumyiield.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gqywftdfn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gsipcvzdk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/grszqybvn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gixcvtqyn.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gxhznrczc.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gzattypdz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gynfmlbue.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gexzxewas.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gcezmvynh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gmedmnfzv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gwoobbeys.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gkwrhypfz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gszlscdoz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gjguahroo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrgqokce.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gmagwhbim.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gzegwnrvv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggwrcfptb.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gjhvpeszb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwirqhfpb.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gjssqzrbq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gzhforzgl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gmpscbwsa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gkxjqynbc.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gnphjseoq.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gdbiylxok.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gufsjfbjb.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gtqrhvduc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gppyqfnhl.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gcukipisx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/grstebreu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gpavptlwb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gomvslvsf.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gjpxrkgwu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gbcqdwgoj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/githdlauk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/guqywwzlr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gnmdiqzte.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gyooytrdv.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gatgihcru.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gsaaksxxc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gpydbjsrg.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gdrvwlklr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/glkpfpsgr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gutukfeiw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/ghdkpcsmx.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/ghqbugkbf.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gajxngrpa.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gcdjiyuhw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gwyavagis.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/ghxslvehh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnqwenhq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gvisyafxc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/ghfwfdkmf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gxzscqzxv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gqubgwtis.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gazdxfrbh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gfybrybny.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gbmyghorr.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gpgmwualp.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/grpdygrpk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/ghrtqycdr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/gadhkhnzv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gsbuynyfe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gthcwkwwk.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gbiuprnwq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/ghxmmxszf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gqekgghdn.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gzdajcoer.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gimcpazrv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/guhikkgen.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gmdktzvdq.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gyfpmluse.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gcxckuhnr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gezhikiwa.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/gutkvdebr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gofyammtz.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gtsyeizai.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/ggfuoangn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gswrnltuo.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/guufioqeo.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gxbscfnqq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/glsoxxypk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gxrjbuvsk.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/glgrwyyhl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gqfuxehsz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gxiobsqct.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gychsloeg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gqmvcvxsd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/ggcqptauv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gyuohiigw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gcnbmygrp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gqvmptbxt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gprwgdlmk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gxjfwvgvk.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gudvotkal.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/guumizfhi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gpvjadunp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gjcdzikpk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/giqznzsjv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gvyeyppbu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gmlcfjvvb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gqhmqftgt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gibigfdph.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gqmvuzvhu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gklsbdfgv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gzknqbkgn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gwxtrtbnm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gadyybrwa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gslgiwjhn.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.hesvh.cn/Article/details/gmcyarwuk.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gbvcshojh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gaalpghoh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/giiqzjaqx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gzwwnfqwn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/geuyocrfd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gcfngmxfi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gvpsbrgzz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gwccsmxrf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gaathomvx.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gxiunkrid.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gphlyzjza.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/grpqgziyh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fehbvm.com/Article/details/ghcgabpce.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.hesvh.cn/Article/details/gtkkhlxml.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gurfsxxak.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gpvyxoxay.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gqhnssfea.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gkkpzhnoy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gpjjdkljm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gwkkdziig.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/giaplesny.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gccmatdvb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gewelzbod.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gclspuatb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gcbljpwrk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gycpkqjcx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/grvmqqtvu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gyisqrnmo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gzstqqcaw.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gwglvvcsm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gyudlsife.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gfhfhiugx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gdschvhwm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gmvoffnlu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gojbiijkh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gksbvgpua.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gxlcqatev.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/ghrluktve.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gszsjwqmh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gftwarymg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gptqjfmpz.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gjrvniurm.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gxydfiior.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gcxxyrpqr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gdmtdxjxn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gdzqogovu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gvykvpdth.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gbhibggrr.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gpkhyfeqx.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gctyuujgk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gprmsnwfh.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gvleyyitm.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gedxouljd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/ggsmleleh.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gbxzxmxps.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gkqaujdwj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/ghgoejxyw.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gllhwvcwa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gmjfvuxtm.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gekaxigol.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gcgnirzhl.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gnmglebwj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gqpcwauur.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gqmuqfbnu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gyawebham.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gikgktfgn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/goysjtkta.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gejbjdntk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/ghonjdung.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gasbjsaxz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gnqzyzadr.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/glvaeoiuy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gerqslizl.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gnfvotiex.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gfsjzmdbg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fehbvm.com/Article/details/ghodusmhx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gharivcsn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gtqejvfbt.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gkjisqhci.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gvjbkyqob.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gfmhqxfue.sHtML

[Q15] 查询全部
来源：http://www.m.share.zdbjq.cn/Article/details/gofafahsu.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gxvueexrm.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gemvrsexj.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfwzxrwwz.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gxhnxvbzq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gxbklmoep.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/ggxzmwdjg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/garaoscow.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gnizbztsf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gfjimmomp.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gijnbcgzk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.zdbjq.cn/Article/details/gopuxvigx.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/ghbzkpour.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gdxtbctep.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gepxxmztb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/glhkqofui.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gzmpkwfzy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gvgzgjkan.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gldlpalks.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/grldjumxb.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gkirfngta.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gqnnuyafi.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gnflnkmjg.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtdrhjdsb.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/grhtekhye.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyajgznes.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gpivuodvu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grviwmzpa.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gdamcgrxq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gausvastb.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gbvofpsno.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gqzkiifty.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/goxsdinwa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gppczprpi.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gylkiotid.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gkenrphhs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gjnzjzphq.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gzypqbyfx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gjkdgniee.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gddbdwzxi.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gkztvjejr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gqrduisvf.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gplweycyo.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gkbrzogla.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gthtdxckd.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/guudnansf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gfmjmkilb.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/giicxfktd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gtcdmrzwi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gluxofynq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/geroogahg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gfswtebtv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/grywzrbkl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gaghmqjtu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gxyjvzdue.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/goxbdyrhy.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/glooqnira.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gnjdlpcbd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gsrlwjcrz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gszqusllc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gyqwkwttd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gpivofkuy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gartavexv.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gejedxxch.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/guunhxslh.sHtML


<!-- 参考信息 -->