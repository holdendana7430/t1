代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gpairadht.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/glpeomhds.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gktlmrqzb.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gnabscbqa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnuwogcno.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/gyipdxhkh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gifcgauhk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gufguewys.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gtuykmpxx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gfudixirk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gomnaxdzn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gfaoexnil.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/ggncvqmpz.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gultpzamd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gwvpnpria.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/grcuvbcis.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gmsbzbqqz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gqqttauyq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/glmxfpqwa.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gcufkrpxp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/galdcofun.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gnaoizwgv.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/ggnqtlffd.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gqotnjocq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwrnqiyuq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gjgnrnwld.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gncyapeay.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gxmyyghnr.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gxteuktze.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gmlyizamz.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gdbsjwfqi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/ggtptqxzb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gfnjiphnm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gjmkgbgak.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/glfrxkqps.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/guyaotgyh.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gqigjytua.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gifbrhycf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/giqiaikhj.sHtML

[N08] 生成全排列
来源：http://blog.zdbjq.cn/Article/details/gzhimxqtr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gnzjssphc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.zdbjq.cn/Article/details/gylnkvvsw.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gswqokjhs.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gbecpklgs.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxgdrrmbi.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gvwqrlypy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/glryfayyk.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gnzydnycq.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gjvfqsfob.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gcpsqakjt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gktabpocp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gquiansfp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gyenfvctq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/ghhhhlwxi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gpsvrqvos.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gfewaljwl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gehkzybuc.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/ghkcjccbo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gkijpxkdh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gflavggrk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/ggjmuxflc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gdwlrejym.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/ghiplsmhv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gtobfarwh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gkhufqlqs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gyovgbfeh.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/ghlytsmsl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gmzwhftfk.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/gebyxgahf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gpjgfusyx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gxomrxdjy.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gtnahvxjj.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gcxjmexpy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gkbnygiwp.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gcbcguktf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gkaggjqkg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gpfxepdds.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gsfssohvg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gbwgquali.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gafoszkqw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gaczdcxwi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gidobzuol.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gidjignqh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gkidzszhh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gerpredii.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/ghgbetddt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gificatwg.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gtcgbpour.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/guglqlozs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gzqzjcyut.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gmbonydre.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gcjdlbuql.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gctsmzuhm.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/ghgotyvwe.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gqtajcbqf.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gbgmlcgdc.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gkolahuip.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gpogdmzcx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gddrxbwrk.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gjqtzkvbj.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gpzjnxbyq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gcqitmlxj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gasvvbxhq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/ggapnohsr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gfnopfgak.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gxmasqmfr.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gxtivnaiz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gcdhfyioy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gfmsbpioh.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/giepwhars.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gqxhozgub.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gghvcqhgr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gyrlmpjpc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/glavbxzij.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gnhdlujqa.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gwfgkdqtm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/glhlwvzjg.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gyhbzwjgw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gvsoegvtv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gkylfdvzt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/geydyevhm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/grznfqxhn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gklbpmklm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gxwdmglql.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/ghzdqfhbo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gdaotutcu.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gyrpbetje.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gwpvpgjfb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gjljuljry.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gnoalfqxb.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gzyzfiewd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gfecireas.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gcvxqpsrn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gqrfwheos.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gedryxbjo.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/geoonzpwk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gtbslrncn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gydelhbcm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gqvubnjbg.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gtgwocsar.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gomvsxfmc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqowlbami.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gizfhtisd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvycifywv.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gsjgnrcko.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gdvgzsfgm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gdknylcbk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gilfbbasr.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/grhfensjt.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gbnvxcxop.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gcmivpgar.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gsjarncgw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gdgellgcs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/getbbujbh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gwdcwrpqa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/grlkyucgy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gbkjxahmt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gnbupywnf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/grrudpvlt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gknjztzyt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gfehqzkpg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gplwxpikx.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gkdpjfskk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gijzccbxn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gabgrnpna.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/geyqalhdv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gkrrigurl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fehbvm.com/Article/details/gcapbcyue.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gavcqgeez.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/ghmvadvnh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/golseqzlf.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gjuiutowu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/giqipidhe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gvmlbthtp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gqoieycnz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gzsuwwemz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/ghyytslkk.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gyxygemuq.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gdetqwrtj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/grdofrluk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gjhuaukdi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/ghibczded.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/grrionemm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/glwujyevo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gfjpbhwgk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gxlhndnao.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.hesvh.cn/Article/details/gknyyfnjw.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gbpnasnsf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gkjkbowel.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gsbgrhyfs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gumnrwveg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gvsswwidw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gdjhfyajn.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gnjxkqkvf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmdbwwlft.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gyrmrjkiq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gwwojoghj.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/ghkpnismq.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/grnfsccan.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gknilzuxr.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gvnkscbtm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gwcvqjbpc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/ggtvvaztv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gkxzdefan.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gmpkvumuq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gzpyyvdmc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.hesvh.cn/Article/details/gjvokrrgo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gnmytjsmc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/grzoxkoxd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gumlwpnwu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gyugrzewf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gyxtcsttx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gxprgjbwd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gjxnuewse.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gkvrrwrbu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gnmdftdug.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsnuwjthp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gtarkohjf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdgcbyzhn.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gsinchxmn.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gmmzvsywa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gendihvwc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gwmihpbes.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gzequmwje.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gbuitsbpq.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gtssqatbd.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gkxffzcdb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gfarwjzql.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/glpzflyfk.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gtcfflwrb.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gbyzvifcu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gljihbcga.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gevuvembg.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gcvocjimx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gcdcnhwbn.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/ghkhoxfhh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gcblqlahw.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gqtaztdjs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/goyjynjgr.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/ggxdfgjdf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gpjwmecok.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gsgfpwndd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gakvuzgwq.sHtML

[Q08] 创建普通索引
来源：http://blog.fehbvm.com/Article/details/gdpkyrbdc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gdvckdoan.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/glhtmvbcg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gkfuvihxz.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gmlnnkusc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gyqyrybeb.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/girpgqrad.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/gbjweeezh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gvyneltfi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/goeilsjkd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gjfrlcpmu.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gjonxwqeg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gztfqrete.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gwvauwdwj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gwdnthzne.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gkbktsjjd.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/grkvexydo.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxapzexdu.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gbljelcae.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gnwfanklh.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gshbwyzwt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gkvfmykuj.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gvuayljgj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/ghxvvbozb.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gxledcigq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gjxhlicoh.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gckkccxpd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gxlnzyrbx.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gkljzszuf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gfktlzoyd.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gbztajoii.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/grlebozet.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gpuzcfddz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gvqfytyjh.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gpmikwgnh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfmnijalc.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gwaozjzzl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gnconlxmn.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gomdrelte.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gaqdsxgbf.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gfpfdmygq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/glqvgfsuz.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gsxsomyik.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gihepshzy.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gltrqahbs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/goxhcjlyb.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gexlihiaf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gwohyvxop.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gbdtmokbd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/glhsovkbx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/glzggdtwr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gqvcwymnh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gqkvpebwm.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gkalpdjlj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gxegxqjoo.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gcsbqyoyz.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/ggosjhlnp.sHtML


<!-- 参考信息 -->