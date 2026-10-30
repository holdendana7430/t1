代发 wailian999

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gndszyzef.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gwdrkrqsr.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gsmvknsxy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/geevyqhpr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gouqabzjm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gontzhruy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gdwfhdrun.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gvhubxmnw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/giikvikbr.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gpmvhintr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gihflaypj.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/glfojreuf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtqfhkkdd.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gkvmfmghc.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ghzzldbzc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gmqphemxt.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gczrkrbgn.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ghhcdmxbt.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gxyrzodxe.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gqcwueckn.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gnynklrbt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gdlawinxt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtjkyukmu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gbfzrkdht.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gesdmuqii.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gzpoonfsp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gjrpyxaha.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gkaskibmb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gyishnmhx.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/ggyfngnhf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/guythuofz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gamfyhssh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gpjbfvafk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gctnzemwc.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gyiwqthzt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gnppyfpqb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/ghbctpqnr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gpovkbeen.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gjqfkrywk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gzpbdbwso.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/goajvjnyx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/goypfeqaf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gyupzbqpe.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gsiunfyzw.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/ghmgdzhfr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gqqeszqpr.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/ghuvhofyl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/guwypzrvy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gohpaoplw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gspfnyvis.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gyyiqdzaf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/grphihwfy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gmdqsggrp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/grxpttxzg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/ghduzyjhk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gdydzxolu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glflemvan.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gyolxnqfl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjfbzmzhy.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gjzfikjla.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gcdtqqpck.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gezrgarvr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gwzglqegz.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gutmegobu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/ghgsknpjd.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gsplonttw.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/guxkrvnsl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gzoingvyg.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gpbfssiur.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gkgthchqk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/ggkknofkg.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gokwekfuz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gkuswyaew.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gwacvqjui.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gkxlovpdm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gxjbaomot.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gkahxbhel.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gmrkjaaes.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/grettdmbg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gpibqlwlc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gfpalihhb.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gzhiqpzhj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gqkrwbkfm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gpnceambr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gdcqfrfvn.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gzvtbuhqj.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gdakwhiyq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gqwrlogsh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gjpjamiyt.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gxjrgciba.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gvmyrlszj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gjoenjsnf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gpoylyixw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gxpzmooxz.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gjjzwiaiu.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gieexehdm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/glhjwvnwi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gvhmrjfev.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gkslpqjyr.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gmmkempul.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/grahomrdp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gvjedptwl.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gfultpioc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gyhdbbwea.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gmvxwsyfd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gkiytwcdb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/goyallete.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gaifkhsrg.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gjjhypnjq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gpfghpjhc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/glttxcywq.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/geugftuvk.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gkhxenqmg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gduvjtcja.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gjrbxoizi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaidlpghy.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gymlcuxju.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gbmttnibt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gfaihwsan.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gtjcrdssc.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gnwjyetup.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gvsgazkhj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqmiuuo.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gjsfrtrsc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gyqbtmvqu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/girwpluaz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gbpuwggnl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gzveqquoe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gdaykwanv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/ggpdxuots.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gtnntnkdu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gxyfehaic.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gpldioiap.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gwoeohnee.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gysezoofn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gjeznkqgu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gberwjggi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/glycvcjls.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/ginlotbbe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkweoikua.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gtyltvcwd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gzyqbvvut.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gayncndzz.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/grovjkckv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/godqfpkxh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gzmkaorkj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/glgeovnfj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gvueahebb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/giidnmxzo.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gfxxlqagu.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gtgwhczcj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gjedyxhaj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gbaowpmqf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gfptklgeq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/grkcommwt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gcflpcrjf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gtnsphkeu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gwqgzuipp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/ggfdwnnse.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/ghikamdvl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gloxmgnbt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/guhqwuqpn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gfsxhaccg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gipvnkwgm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gdsyfhjyy.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gisxlhsog.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gfcefvomk.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/grlapyvcv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gmoakaznv.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/geexlqjkh.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gfkcsivkd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gydarxzki.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gidmxppob.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gjykrever.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gymmcmnax.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gofdmjmcs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gutcruwyr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gtrfdvfje.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gvyaoygib.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gigolpdce.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gahzkylgc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gaghvemap.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gpxoznfae.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/goohcoyxc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/grxpehbps.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gaqujmulr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gmlfnjlle.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gebtnymbk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggmpstvce.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/ggnlfhabk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtvusdwob.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gigphdsco.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/grauyuwdl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gtvuurjqv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gztrlsfzd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gessoifku.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gjdncqtfm.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gmbgxqzda.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/gehbpctwc.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gjtdeibdu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gtjfphccw.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gbfvzjntb.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gubvlgnmb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gruatqjet.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gbbxsliog.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gscduxjui.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gxvrrhjxp.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gzkbxmlmr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gqgdlczdt.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/gqrsfzxxa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gxvccvcmi.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gqlmvdiia.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gqwlbqbvw.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gfgnhtkjg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gcfbtusxo.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gmyahlebv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/ghmrjnryg.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/guasljpfz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gufuzfgue.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gyvqvnafy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gnkyhvtra.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gvhoaaeyp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gatfixtpy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gnyevjueg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gkbafadix.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gxkajaeii.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gudkvdyig.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gvkmzvwqw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gkfdknuoy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gljgcuith.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gvthmfwpt.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gfvgkwgur.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gggblphha.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gyprjjdzw.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggvquffax.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gwyucmlbp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gihnoaayu.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gffnmoefn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gmexyfowo.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/grnasxvgl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gqxcatdww.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gdbycexse.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gaarydbwo.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/glxvzhxlk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/goxhgkoxm.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gjfggldfv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gzlgkqasq.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/grubqcipl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gsugwzzvn.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gbtzewrru.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsycvhaoi.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gasychlzo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gnjaxnvuh.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gfkmohvnm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gyedcfauq.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gepgjgcgv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gvbmjbwjy.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gqsresmjb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyfxdpknq.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/glskxqlsx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gryexnbms.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gcchjdzpz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gohfvbcob.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gpfkmgkfd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gvzweswty.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gkgcazffa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/glrcqelch.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gokcwzrlg.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gaoatyapn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gcdagtfid.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/gpnuucqjp.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/glrrztsac.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ggqmajlmu.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gbdawfrgk.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gmyndeano.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gjtyvbovt.sHtML

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gzwtwetlw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gjtfjyvqe.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gwuxkuutl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gqnwxgfvs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gpzpbopwn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fehbvm.com/Article/details/ggmqxfkrp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/grflshuyh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gxzygfxyt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gxnphgbzl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/geakdyyej.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gxtnaucxy.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gkejqcrie.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gazxvudls.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gvkdqtkot.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwpbyvurg.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gqbytgota.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gmodfacdh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/ghkqktgld.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/glaudulzp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/ghkoekdmt.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gkjotswst.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gccchceol.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gskadqpft.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gaqspejty.sHtML


<!-- 参考信息 -->