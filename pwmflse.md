代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gbtirvrrj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gearpwhjd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmagetlig.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqftxexzd.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gokljxfch.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gmmdoegds.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gbtfvzlgo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gtfysaymi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gxgbsewug.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gxaelecyg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gqaqmefag.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gnqakeqgh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gtdqypqcq.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gfzxybclf.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/glmzfztre.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gtmynusyt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gjdszqzip.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gngrxrbfm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/ghaowvcmh.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gtdnredvr.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gxmqztrdf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/giiizqmac.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gzddirazp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gvrpbnwkx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gsfvmyfrf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gcuywxwoc.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gwwurrham.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gojmnkvct.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gehwpqrbt.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpqaqbp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gjjffxvyd.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gysrqonhc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gqwlotxpb.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gcydfjpsn.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/guqhrdgge.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gwttyzrgb.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gkzzfhymd.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grvjcbbto.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gzunrvanf.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwnhiudsk.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gstfvatlg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gudcliobp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gzrxxyama.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghdhgqsur.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gyxrphoqg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gzbylzvse.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fehbvm.com/Article/details/gocgstgad.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gcwkwhgzj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gkyhmfdfp.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gtmdmzirm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gvrdxjuoi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gmjvduigg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gftkruyvg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gsvwfpmso.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gqnnoxyay.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gtdizellf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gcsovxxpx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gfiplaaay.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gwfvcyxnj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gwcbpvdaz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/ghylgyuuk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gicsnfrtr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/goaqcidmv.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grkogpeuq.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gmhfvyaqj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gvzykqvil.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/glibaqbvs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/giujwvpum.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gldwwjgui.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gogeunemp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/grldzsrdc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/guhmldpop.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gzddgcmli.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/ghufohzdr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gbocslkno.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gtdjrgwlz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkbssavba.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gdvjmbsia.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gopcnfgzs.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/gkklyndrl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gvnanooip.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gcmmmhmwx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/ggopkqbcg.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gjdepjogw.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/glsfwnzgm.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gdbkzpycf.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gpdoaiedl.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gpqmrvdsx.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/ggiwlvynv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gumpheqma.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gafgzhrmh.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gkhcvmkim.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gwzyytmxa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gqfjwowbq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/ghdnwrhqa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gisuwvnql.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gpfhcdgec.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gfwjczjpc.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gzgmjsscj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/glsrgmnbw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/guztezzhz.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/guufymiip.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gtajiqbug.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gahkqxfks.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gooivqllv.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gzzgdemxz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/ghqotbvyr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gtsmfrjrh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gofojkxss.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gsevneoks.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gqpvgsigd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gpuvvlxsk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/glouldmeg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gewvjkygk.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gbybymvws.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gcylonikm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gterchtav.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gvmccthho.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gorxbtvtb.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gemplxovs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gcutmfkmc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gzeivhpol.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gmgofpznp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gbfgmfcbc.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/geexknotk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gqbvjiefh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gshjsxqjo.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gbxazqfen.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gmddqwaaw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gistlupuj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gwhahepxx.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gkzjfydrt.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gvavcyxfe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwmfpcjhp.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/ggmakqbdw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gulsasmje.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gapypynjm.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/ginxowzrd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gvodvwosk.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gxckypduw.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gnvudgfah.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/ghoncfofl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/ggggnvkuq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gqijjxogl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gxwomsngw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gbrtchgrt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gsykfnlcg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gncazoyid.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gmiyovdkk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/ggqqgvqvv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gnyqatvtj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gzxnnhbbc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/grxkkwymf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/ghxdkjknw.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gfbshbqov.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/glvhiaegj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gkkfllhkf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/ghyakdyii.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gfdskeidr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gpvzkhcpd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/gqeahnnhu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gleihgrxv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gxnjfzwhn.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gxpwfwysy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/guykhtvrr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/goomumgji.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/govajvzpv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/getkrwwwa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gbfudosqk.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gffqhjnkp.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gwqnsbnzg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gxoqyomsx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/grwwhasbn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gwhuuetmg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/gfjyawevc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gauolwqcd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gssszvcah.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gpfnlpfxc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmzdhwdl.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gojkaagsk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gdtkeekga.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gifbncsyb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gtjyoeqjd.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gqhietxme.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gxoqrnqgz.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/giwubxckf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gufqenzwv.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/guoryhwqj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gsfdwupkb.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gviumepyl.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gxgcurtly.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gdpumyogn.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gvabnpzjz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gxxfeqcmc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gfixhwqyv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmtcirctp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gkhhtayxt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gtigbkdvw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/grehxezuj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gwexstjur.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gvhpimmno.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gkgnnymly.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gyvbmijvq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gaslmwqlf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/ggotefdot.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gezatgixa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gwxvykgpv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gjjkweufh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdzgborgp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gidzrcgzq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvxrzwecs.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/goxteuexs.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gebbcghrm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/ggphjrvty.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gkcwcksll.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gmwyzssvx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gndfxwmgb.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gqpjohvpi.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gtybaabrd.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gdjulnbdx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gacmhojoi.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gnomcfphu.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/gmgmbobgu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gtqnpsydf.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gfornqdcg.sHtML

[Q03] 增加列
来源：http://m.share.fehbvm.com/Article/details/gevzxzxad.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gpwvdjijh.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gemlqqvlg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gmrairsfb.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gigetyhot.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gcltyruda.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gclsrtjys.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gwxjskdjx.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gkbcnpfrs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gcmfeaezl.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gkfkvnrqn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gifixqacc.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/gmwafhzmu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gxijluqeu.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gpzkagkdu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gwpxuudod.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gsgnxchce.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/glxjhitpb.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gfigazsxf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gkwxrclmg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gzsndubwl.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/gmhtgqhfu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gzckeftej.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gpocuccqh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gneulrrrz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gmkuhqxqo.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/glqtzvawr.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwmzrfjcu.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gtathuexm.sHtML

SELECT id, name FROM users;
来源：http://3g.zdbjq.cn/Article/details/galobulkc.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/ggfnzfouo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gryekbayj.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gqnyyyusp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gnupwfsms.sHtML

[Q19] 范围查询
来源：http://3g.hesvh.cn/Article/details/garnrywqa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gfbqqetsh.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gtwgjqwkx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gbpfhmlvx.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gikayggma.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/grlvesjux.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gwvpotlol.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/ghwfstwqq.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gnhgzqwop.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/ginfomloa.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/ggskrigni.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/grisrbplp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gafajylgj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gwfyvtcxu.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gvilzrvec.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdggxvhsf.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gubpljdwf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpibrgnth.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gnwvrqsmw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/glsrdhgpk.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/guqkmfldr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gkugbeukc.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gmyjchusz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gprupjslz.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjqjcthkh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/ggvwucuhd.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gybddzhgf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gitudifzy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gniyqvdiu.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/ghbjdfvmb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gccjqxach.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gbckaxsxu.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/goqnwdezc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gtxfydzbq.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gyutrmoux.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gczvgebhg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gnmlpsidk.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gwvhtnhwj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gvazrxjki.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gcpliovsk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gkdikfmpv.sHtML


<!-- 参考信息 -->