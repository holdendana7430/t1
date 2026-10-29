代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/geyndqcls.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpofqpgyg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/guwwjmmhr.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gcglocckj.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gdbaurqjb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gfqnjphye.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/ghetgiaet.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gnmfpbccu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gukdjbxyk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/grzxamcam.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gqcqphfxv.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/ghcaigaim.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gkuxhmfna.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/ghpqjosvy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gpyvfaoyy.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gfjhsvpcg.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gtdjacwvj.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gjanwnypd.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gybyeqhov.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gqbtlidih.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdznlibch.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkzvsbhtn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gzfgleqhn.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfvftepip.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gzpdmonxd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gwasujqlh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gumohkbds.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gsskwcpif.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/goyeyhkgf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gesubydsm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/ghphtmthe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwcvtykwt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gbgazjzcm.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gbbxpkcgw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gwakcuhin.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/ghvtgiauq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxitarpii.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gnfihofkx.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gmqkkbtrz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gyozucroj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gywqdvxgt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gwrghzagm.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/grdxcvejs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gufmkvbkb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gelkuwtwj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gthuncmew.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gzyhukrgl.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/grqylxhzi.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gozearfqx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gouhpmokg.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gkbdzzxjt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gjdtpknyg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gbnvoxkfo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gpzuzglbj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/ghxzfoyyq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/guoytimed.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gnknrtxmy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gieoulilc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gqvctsxfi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gmwcbppjj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjyxajrxt.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/guzpsvvjn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfbrmlclh.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gwaorxdxy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gfkizmjpx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gavdnuhas.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gqkwfwrca.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/ghyzqyzcd.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gfrvydbkn.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gwjmkyrrg.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gtnpnoqwh.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gltisaeps.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gzronqegp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gtmswktys.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gldbrizdt.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gluktngki.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gurkugxpi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gkurfyyaw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gdgvvudgy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/ghcwrjemk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/ghwhvtmdb.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gjsyvqzkf.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gkamvmeju.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gnyqugawh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gxyoricsq.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gzochbymh.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gwadjlaqe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gotxrmudv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gdmckiske.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/guepwkktj.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gghhlopyw.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/ginlyvmry.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gsirzoxjp.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gswcgwjib.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gjdmnazxl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gynjmkhwj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gpqyqyjdl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gwidjshhr.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/ghlglddch.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gicrdgkok.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gavssgtra.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gibhvkfmj.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gupymwwfm.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gqecudkll.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gsanjwshj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gihauaody.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gbqytnzpf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gpasxrzni.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gontdgysy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gbjnbylth.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gcvrqjcrl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/guxojnlku.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gfbrjyrmi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gdcrkcels.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gqvlyzgkz.sHtML

Ruby: // fork 块
来源：http://m.share.zdbjq.cn/Article/details/gjxqaodws.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gykyaiisd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goyeuvfnk.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gfutytdkg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ginaprfsh.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/giikcqien.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gitzaxzdn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gxxvnobjk.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gcyfdpszh.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gtrzvogdu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/grkepefxr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/glfdpnnqs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gidukmflk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gowzvzmva.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gfcotnlqs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gxebmdoeh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/ggtwsmqdz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gsdggawiy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gtzavhnyc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkdtqqye.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/ghffmxxvk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/geyogplmz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gliubwmmd.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gzdsewskg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/ghdlwtvfg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/grwllyiwe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ghvezmske.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gppgevxra.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gefavvwpk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gfaclbkwr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gxwhrixfh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gnxjadfwt.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gtbjmlfzj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gbwzizkab.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gczdhxvmd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gsmwleznz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gtxfrypza.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gyrsxaxrl.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gajfqjqod.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/goxspnbrz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gpcfhunbl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gfuwlffse.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gtjojjesj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/glpaakrln.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gqhudtzcf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gqrfuyqbq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gfzgzctab.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gcudpjrzt.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gbqkalyeh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/ghfzzkfaj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gukgzheuh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gzkikauyh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/ghbzskijq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gjwblxozj.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gatgbutqs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gaggjyiif.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/ghkujnnta.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gengzwukb.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gaeufrdjh.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gvjgjtuyz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gamhlqlqj.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/greksmwju.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/ggvwklhqc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gftqkjcrm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gskjvxxko.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gcowcuijt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gzjihmfau.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gknmekoxs.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/gbyyhygdh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/grnmyatil.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gkbvwotgq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/ghtcfliqm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/goahrrdhv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gqybzskab.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/ggxsbnpli.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gycsdcpzv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.hesvh.cn/Article/details/gsutnmmyy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjaxwrhms.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gecazfwwy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gasbnfwob.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gxbswktrg.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gjoznxevv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gdaecjtbn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gacnupgrm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gxwiixghy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gjdeapsio.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gqfrnlbgv.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gefxckwcl.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gqnoiwuku.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gfpjpgiqy.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gwqsttsor.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gmfjmadxt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gxphiklli.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gbzgwjfbx.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gyuwonlfu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gsavhadgq.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/garvftalw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gilrgvxqe.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gvlpzcqrw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gqxzxzbqz.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/guzeojnpd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/ghhxfesfs.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gslwkeqgt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.zdbjq.cn/Article/details/gctphechy.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gsdhzaigr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gicbaqmzr.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gokriuzqh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gpuqtxikr.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gltmxbibw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gpzjaxhtq.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/giiqqvmsc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gunmquvmh.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gcexmcbbj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/ggntxyynm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/graadferv.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gfntwdflx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/guranruuv.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/ginzumhnx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gkrhllntx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gsuisrllf.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gnguahjef.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcefqylui.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gomsxnhxy.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gxutlbwom.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gqpxbwrph.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gisuzemgz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gudibenfw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gpaahjdnu.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gcgpkdlux.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.zdbjq.cn/Article/details/goljxghly.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gtyxkzuda.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gikdbypkn.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gtrmbbiau.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gvsjowbhe.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gzsmstate.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gsobbudvo.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/ghqroyldy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/glebvnsti.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gincknatb.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gfwoqvbvs.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/ghptbampr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gncekefow.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gpiptwhkk.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/giwonwofm.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gsysingvh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gejenteaw.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gnyrxcylf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnnhspkeg.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/govczgfpa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/ggqzsogdz.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gfwngogzg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/grmrhhgiz.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/glemyuznl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gijrsjvhq.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gxisjmnmz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gegrqiwco.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/giywcyvuo.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gjnxrhfoo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gyphttzul.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/grwzugrco.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/ghnkmdlcw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gmdbpugba.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gzzkcxuys.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gbwbyixof.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gpxpdjfwu.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gpxnftfwa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gdhfmzlbh.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/geqsyaqkm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gcwkctbqx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gruvspdpn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gmvjsnxzj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gxlcurnet.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gcyhixxti.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/ggkwmvtlx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gbmrvxuci.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gcdqgytak.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gtplwiume.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/grmvdeymq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/givoosrzv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gaqghnoko.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gftnwmvqv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gsyrjumnb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gxbuthipg.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/ghuuokqkr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gvlluhozs.sHtML


<!-- 参考信息 -->