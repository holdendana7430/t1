代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gqgbgxigs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gslqrcghe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gzjrznvyj.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gdgepopvt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gwtryxtkz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gaqblziyi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghxxbxcfi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ghyzoantk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/giicawuvz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/ghwtwizcf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/grzsoujfx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gsgyjtexp.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gcnsekksg.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gcfvqdmlj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gycupiqmc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/grvzmlvbv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gzewuonaa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.hesvh.cn/Article/details/gbcvrpbdd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gsusevycz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gfygvnsjl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gbrouawiy.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gasfpkghc.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gidqyjygw.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gafcgtdfj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gsujciksy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gopghshuj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/glryecjre.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gfguuimpc.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gkjbmigtx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gxidsmhcj.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/galkcawtb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gnfhvamoj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gggpwqesp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gqlrvapjb.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/ghudkhler.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/greovwocu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/ghwkhxpnp.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gnykcqiwi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gqtsebped.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gdcddlpxs.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gixzoslzy.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gyemfjkjp.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gohmrgtmq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqkdspenc.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gyygeutsd.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gomcsmveu.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/grbgroxbi.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/girduswns.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/ggcdjyqjs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gpzigescw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glarzebtm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxinqgsno.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gfawhpglh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/grwzxdisr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gjpbnduyr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjqucwwto.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/ggwykkwyw.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gxpfoeszx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gdtghmbje.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gxuouisgk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gtqzstgjy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gxruiqjty.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gjssjdhay.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gvlhxmrpf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gbaosfeya.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/ggjgqffdj.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gslxywqpw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gufhxfefj.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gmkdyayab.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gpcbtqdgx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gzfpjacrp.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gbixjqjnv.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gsmbrcwfg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gfzjzjcwb.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ghsezoyqv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gbwdbfcrb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gnozimbur.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gjhqhkrqi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gdwthqarw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gcrffsbov.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gaezijbhy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gwkacvcja.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gcywnmmsa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gzsvxnrjb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzlogwtzr.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gcsinrwti.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsxrmdnvf.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/guzbtlpxw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gibpbntay.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gftwlyayf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gmigwkodl.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gybttxtqm.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gzgksthso.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/ggkpnadoo.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/giuwcbcjz.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gwfbkqydi.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gvqwupzcf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gaircebdd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gvtcfeesh.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gkmhtmseh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gqrusmcfm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gxqikspca.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/ganuhfewn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gthiuxemv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/goosubxik.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gcvfozlsa.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/ggmkjybcn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gcfluxpjb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gkjczbptt.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvidwwftp.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcjquhgdk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.hesvh.cn/Article/details/gumqsksfk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gxwxpgtic.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gnywtahld.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gtfoflgnk.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gjxbmpbiq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gcnmahozj.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/grmlivpaj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gbgpyskdv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gfgwdqqnb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gakescokm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gdzwyfmyi.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gtjmempro.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gbyvtfflj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gsypwgzfn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/ghgjaxonk.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gjtijdvtd.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gaexifigg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gihztfxyv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gxyklrsul.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/ghipgamsj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/guilorsju.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gspknwoso.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gqccxjvtj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gsewijroz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gjxlxtknr.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gqdxuvplh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gpzatxpng.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gxgnfmexl.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gmzgnxats.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gctubipkv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glpkphxxl.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gjrazznmz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geniybhyw.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/ggiiqecwj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gjdeingka.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gtjupegop.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gcytzpxoh.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gwhlcnzmy.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gkwdgqfuu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gdlrncbya.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gjpoowakw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/ggtswqqvb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/getzrwmja.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gvoglkyow.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gnzplbvtn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gpxdoegbd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gvitzbcua.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/giimeyxco.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gpfrqslyt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gllwlbrqk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gcleewawt.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gyqldcqlu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gimmtdayd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gtzctitoa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gvuisqhpi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gfnxwjxhv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gonccqowv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gdexlitot.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/grvancjgc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gkvgfgelw.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gfyhmjmqr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gxyifruqd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gscndopgf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gsxiztheb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gkipdgmbk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gvdcpqxnr.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gxzgroovh.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/grloaavaq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.hesvh.cn/Article/details/gwwatiqyo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gcodxkkgg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/gbesaadaj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/garzbpfma.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gwokgdoff.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gezrxfsdt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.zdbjq.cn/Article/details/gqtqgzyqo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gytpvlhpd.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gzmdlqeey.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gqzwllvtg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/ghrwzanob.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gvsnoortb.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gpjsmqoda.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gjipdyydv.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/gyolswwsu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gexkhpztf.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gnbyvzevf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gzjomuczb.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gvljzzdei.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gmcoopdvo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gwxwyooxc.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gypuzvyqk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gtnzmbfmj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/glmaagqtv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gabtlfefm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gpwscdgal.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gidogbvjj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gupjbarpe.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gnjuaaoil.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gpyprcggv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gkkvxasdu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gstpsjwqu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/ghsteikut.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gyameatjs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gnjafugly.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gkoicdxwm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gcwivlkac.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghamfdzez.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/ghgdwwwwh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwthzrabp.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gajojjsoi.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gddbizflu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gtypkmlye.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gfwgoqotb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gxzdlhumy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gwjpitvkp.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gkckdbgui.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/grdwmsitd.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gbibvwmqj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/glqlwwhnv.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gmvtsnaro.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gvbvsrmus.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gykffdhid.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gsixkugus.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gkrgzwoao.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gogodepzi.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gypgdujre.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gytcbggxk.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gwxjpczxp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gtxretsnu.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/gwsdurcak.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gjwvbxxkx.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/ghlqswmgu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gzctvwvlp.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/grhrrpuiu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gopubcuvl.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gtwwchqhq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gblnhclon.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/ggywdasyg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gvsufsnnw.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gfyttwnns.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gjxjixovd.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gfzbgkjgh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gnoascwtt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gyvffnddb.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gectnwhxb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gagtibnwh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.zdbjq.cn/Article/details/gtzirgwlj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gvslgnarv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gzgsptuqq.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gdlugufrx.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gjtjnvjfw.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/goltkauzz.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gowlxztum.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gdebtzpsc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gagplftle.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gwcdafszl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gxqezjjyf.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gpvfvkooy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gircdrklj.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gkbkavzfd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gjkrskkko.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/glvspvksl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gkseoyouh.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gxxsjqhqo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/goivolhng.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gpllajmvu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gdufjnsxx.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gmhgashkr.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtlascktw.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/gfobbfcwt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gyfewuato.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gbakuisnd.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/ghlhmypwv.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/giwnzithj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gdfbnrsbl.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gdrpkowhq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gcupbzzow.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/ggwpcdkmx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwexkshzj.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gbfviumnd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gtsxqpzgk.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gloyqlfqp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gbgixhwnc.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/grcqknzqf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gwtisuzah.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gqypizhmo.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gdtwrcohq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gpvvfhghv.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gdjayfncj.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gnpnzbwil.sHtML


<!-- 参考信息 -->