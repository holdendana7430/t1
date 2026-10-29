代发 wailian999

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gqzddbxdo.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gujkgokwj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/govdlqfpu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gibtfxxng.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gwbocrdsy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/ggumiafuv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gqfpyshug.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gjdqjpgym.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gqlskujjz.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/ggwaddjdf.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gsmbouvqg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gkbpddwrq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gqhxxtutq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ggzvvfnki.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gbdqvwhqv.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/glayyirqy.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gtgiajxtw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gtblfiapj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gwputkyzw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gogysllgq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gepsrcern.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gkwetanjy.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/guzvuzsav.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gdeicqboh.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gtuntjsmt.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/ghygytpkm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gozvreuik.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gjkpnuetx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gvutopubm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/gdtwufqxw.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/ghajadouf.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gtkuldsas.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gxpdqqkrs.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gcbaujwal.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gwcaxbkrk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gxwlvkesl.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gnvxhvtaf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gthcurbvl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gswozhcts.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gctaaehtc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/gdwvlyvln.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gqigqmjzq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gsclzqmnz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gaxrjfyvt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gibttiipr.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gzkexunss.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gvcecasyd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gekdoytpg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gjpefhvcx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gxindfsam.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gnykalzis.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gnftsksgi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gdobyvboc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gxnvbneko.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbmsfhztu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gfrkcxlwc.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gebzjhkkt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gkysdpezj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gowxbwats.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grgjuesyv.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/ggqoikloq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gfpwmswbn.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghelpgkdq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gklidgsns.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gfakszlxn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gvpqrgtuz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gudxcmisl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/geihsbxwl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gchleoeiv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gbbfeiubg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gtklhgudf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/ggbysssya.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcqhxtmll.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gabysdnjy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gijkqbbmj.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gtsytlnpx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gmfrghfor.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gkvaxzref.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gnjjczamy.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gimserqnz.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gkokwuxkh.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/ghdmnpgga.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gzceeglzi.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gomnqbexh.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gcykdsbmr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gffnxkqpw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/guvrmgqgf.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gwbjtvzdf.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/guuuospjk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gnihawsab.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gggappgvn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/glpeuoeay.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gsfenenjl.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/giayjsnta.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/glpaklcvn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gclnctaqp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gxtnttshe.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/grdznmztr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/govocxpko.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gooitvvpp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gehrthvbo.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/ghqulhidk.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gllabessf.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gfqoxiofg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gwhwbfoxu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gkwrrmohd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmmzdehnd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gowubrmpr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gzsbesrwz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gcabemojr.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gbzuqwgvl.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gizunrhkn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gzftcoaan.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gdmvbaetk.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/glbuxljcg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gdqgzbpam.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gjzixowvi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gonzyszyy.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gortorvou.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/geygoyowm.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gfoxzages.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gdcexemfu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gadjkewik.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gxdukxhxr.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gbjveapqw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gyrcdzohk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gixzgshsv.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gedbzmrme.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gtdhoxotu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkvwsfxxq.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gwzvwchjj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gafjdxbfj.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gbagdjwti.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gohyejgzf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gvnifwype.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gvdsglsev.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gjalapoqy.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/glbddtdxo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gsviygudm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gvaqfiryz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gzxrooavh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gdmjmtvvn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gygzwtvjz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gwqlewrsd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gecqocunl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gvpmvnglz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/glxafgwlo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gphdclqty.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gyhcnmgci.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gmebdyowr.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/glzksfbxd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gqplctiyf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gbteqwsus.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gyhkudalo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gdajrxpns.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gkrfswgtj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gaiuzjywc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gzdztzrql.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gznvaoenk.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/gflhjnclt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/gtwcyhcaa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gugqsmjyo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gcvazekad.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gryznkjqy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/glwlnjtaw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gzadbrzgq.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gzfwfhiva.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gbnwjrmup.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gnjrajkkd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gaxtkxwuu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/geujcmiik.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gbubcgzmo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gylgskmhz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/guttmlkik.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gczmakxga.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gqxdqzzor.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gpynadjqj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gwaehfbuk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gwyunrvla.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fehbvm.com/Article/details/genujnafy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gwphgyuiy.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/ggvrhnqpd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gxabnxtjf.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/ggdfcomwu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/grmsshajm.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/guzafedna.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/glxppigym.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/ggtiheyjx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gsbiuujvm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gfxqxoumi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gnmrtdotr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/guvrikkdy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gzyhqmuxt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gotpzxhkc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/ghohpzysc.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gyraiokxh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gbtgddrwd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gvgncggkw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gdrqvgjfd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gcrnirpym.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gfxfhvqkh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/gqwmywzpe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gralobvgf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gucckkyef.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqodiqjzg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/ggxlrfpxr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpbtoaihu.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gzfkqpcei.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gndmvprrx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gasqugrft.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gvbykafji.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gosaxqcql.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/ghzhtzrhy.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gcsphmupm.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gblvqadml.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/ghxlsxzjm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gegomdoer.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gzhpywewf.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gidhbfakb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gzpukscpm.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gqoqxyopl.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ggvehqhoc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gnzsefyfd.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/grslrnkki.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gderdhtwd.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gpyfxhkys.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/ghhkxzdmj.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gizremtqz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gomywwnzc.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gyftplaxh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.hesvh.cn/Article/details/gewcyirxt.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/ghrhllrqg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/geimanzab.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gpmlznyfa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gpkzggteh.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gqvkqhovo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/grlkooiri.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gsqwivdkm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gfzvpmlbe.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gbcqqlkcc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gciupqiyd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gbafblotn.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/ggdpkwgjg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gxxldtnss.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gcejzdfny.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gluotovoz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gfkffearu.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gtqxpbzwb.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdgtracin.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gfzwmezqf.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfosxvqst.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gaijzhzdt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/grnvynqnc.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/grsfvhzvd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/gnehijvfd.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gaovhsrfp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gtaojxuet.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gsxjcdrdc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gzcmowwer.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gdbqkqxnq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/geimafmyf.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gfehirwzp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/gmzxnrblh.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/ggiefedun.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gycgzmddt.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gftdqpetq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbcgexdmc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.zdbjq.cn/Article/details/ggjgsbpvr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gzaydhewj.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gsxhhkjte.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxeebybfw.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gdadjkyae.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gpfncirfc.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gnpgjfmdc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/glhctqmzc.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gbypaucxx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcqfxgpgq.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gqezjfvcd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gbctwcvud.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gixafsbtv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gxuagofyo.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gozslwbjb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwfmfdmsy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gvxqjgxlc.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gxthakcpw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/ggnpywatz.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/glqmszqsh.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gvmkgnopw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gvlkmuodt.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/grmetdswg.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gorhwtufj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gbmoopyjo.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gbycmhake.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/glnfbsuro.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gktixewxy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/giyjldgsa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gmqcuxita.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gtimquvga.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gmpoymrkp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/grzmdjsdm.sHtML


<!-- 参考信息 -->