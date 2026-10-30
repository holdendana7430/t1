代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fanxiaobao.xyz/Article/details/guouaigfo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsopgiqq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwelwkyv.sHtML

[N04] 斐波那契数列
来源：http://blog.fanxiaobao.xyz/Article/details/ggnzjvews.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwvyusky.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqgxwezt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gxcimowwa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gbloiwjxw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcjkvlyka.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjsezyjl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppdddfgk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyerllpxr.sHtML

[N05] 最大公约数
来源：http://3g.fanxiaobao.xyz/Article/details/gtitztrsp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gvwqrxazn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdertljv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmsakgdau.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giadssskj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjibsfavg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjsfcmat.sHtML

Ruby: a.gcd(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gabpsbyhm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fanxiaobao.xyz/Article/details/glxoqiudr.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktbjfepg.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gloylvurj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gliaucnsd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/glejawyjy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlysppsz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnrwqfme.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gtgpvakvt.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gtnojelaa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gidimcyva.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fanxiaobao.xyz/Article/details/gmgmqehcd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fanxiaobao.xyz/Article/details/gsnggnuja.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvmuxzou.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fanxiaobao.xyz/Article/details/gcthvnlrl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauctzgtg.sHtML

Java: // 手写 HashMap
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwiwxfqp.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fanxiaobao.xyz/Article/details/gdnqprbpj.sHtML

Ruby: // 手写 Hash
来源：http://3g.fanxiaobao.xyz/Article/details/gqfbhgyck.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fanxiaobao.xyz/Article/details/gksrccuzd.sHtML

[N08] 生成全排列
来源：http://wap.fanxiaobao.xyz/Article/details/gyukjvywk.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gyaaixmui.sHtML

PHP:  // 手写递归交换
来源：http://3g.fanxiaobao.xyz/Article/details/gjaisqyxe.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gybygbfga.sHtML

TS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gfmvutnum.sHtML

Java: // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuwknbxz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicjfvubf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gobljdsyl.sHtML

C#:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gujntabtg.sHtML

[N09] 栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gubwrpnck.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/ggtacotct.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnheltbg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gomcfaskh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gtryttoim.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fanxiaobao.xyz/Article/details/gjmrxbuab.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnrqxznv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gtjsvrlzq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgieuarr.sHtML

[N10] 链表节点定义
来源：http://wap.fanxiaobao.xyz/Article/details/gyzoglqtm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrpsthfl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gabrnwztx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gsjuadjzf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzarokkjb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwtlhpgz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fanxiaobao.xyz/Article/details/ggkpdnwkm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fanxiaobao.xyz/Article/details/goqfcifyw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fanxiaobao.xyz/Article/details/gndrazkmm.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgjmyddi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/gsyvrqgxr.sHtML

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkxdcdufs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfogfammw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjcmpqan.sHtML

Java: // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnksibqqi.sHtML

Go:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmvmovuj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfferqzr.sHtML

C#:   // 手写递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gejiljpbv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fanxiaobao.xyz/Article/details/gqolxinus.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gtplutnxr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fanxiaobao.xyz/Article/details/gicnjjqvg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubmklxot.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlfefvnz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fanxiaobao.xyz/Article/details/gnjpqdsdm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gqfgcvgox.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gkuefzlvg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fanxiaobao.xyz/Article/details/glcjfehfm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuhwuhxo.sHtML

O. 并发与异步
来源：http://3g.fanxiaobao.xyz/Article/details/gzbgtwpod.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvrcxban.sHtML

[O01] 启动一个线程
来源：http://mobile.fanxiaobao.xyz/Article/details/galfjlopp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkekrbosm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fanxiaobao.xyz/Article/details/ggjxkdmcz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fanxiaobao.xyz/Article/details/gwdfiecjn.sHtML

TS:   // 同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbbbtues.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbknkiih.sHtML

Go:   go f()
来源：http://read.share.fanxiaobao.xyz/Article/details/glkarrntt.sHtML

Ruby: Thread.new { f }
来源：http://3g.fanxiaobao.xyz/Article/details/geazcgecu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbfybgjm.sHtML

[O02] 使用线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/grymlvjtv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gytinnehk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fanxiaobao.xyz/Article/details/gesdumagt.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fanxiaobao.xyz/Article/details/gehuxemel.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gkhrgalqw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gumjhdnem.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fanxiaobao.xyz/Article/details/gofbrkrxq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gxkspurvj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fanxiaobao.xyz/Article/details/gbdbjswfb.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fanxiaobao.xyz/Article/details/gbvjkujpl.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysgjlduk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpgseulm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbptfbyyq.sHtML

TS:   // 同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gujphvsfv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/graqtqjpw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fanxiaobao.xyz/Article/details/gbqgrhvuh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjnkeext.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkusfmqdo.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gfhnsgngx.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fanxiaobao.xyz/Article/details/grmwddtup.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/goeiqgqjo.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzshotkt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmalwwji.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fanxiaobao.xyz/Article/details/grdamzaop.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fanxiaobao.xyz/Article/details/gvoxudgub.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fanxiaobao.xyz/Article/details/gejzeqbwh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxujtrwji.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goocndmnr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gpnlyhuef.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fanxiaobao.xyz/Article/details/gfuagwvfc.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gaweatzan.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlumqfok.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/gweqdzmlc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guztcvoer.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfmdfaxb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfgazcuoa.sHtML

[O06] 使用进程池
来源：http://wap.fanxiaobao.xyz/Article/details/gzbadaxov.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fanxiaobao.xyz/Article/details/gttmlbmxq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsgrwgpu.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gadsouzih.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gdqldacul.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdxxzkor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fanxiaobao.xyz/Article/details/gcdebfdvg.sHtML

Ruby: // fork 块
来源：http://wap.fanxiaobao.xyz/Article/details/grokvbqst.sHtML

C#:   Parallel.For
来源：http://read.share.fanxiaobao.xyz/Article/details/giuedcdmq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqnwzhmqy.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggtithgm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxdydwhuq.sHtML

[P01] 生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gswzxmbke.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurkpffgk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfdcucrm.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/giaqlytpx.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gpisgykuy.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gsbccoctq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fanxiaobao.xyz/Article/details/gqexmfqma.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnittarc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpgkkach.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdywmbihh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fanxiaobao.xyz/Article/details/ggachusxe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuusxaji.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gajbbrhtl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fanxiaobao.xyz/Article/details/geeesrows.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgsyubux.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfzupvqn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqlcznhg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtcksrdc.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhmrugel.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmlvhgvg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fanxiaobao.xyz/Article/details/glafjanuw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdxpontl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghclxfxls.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtgcejmu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fanxiaobao.xyz/Article/details/gkeowibpy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fanxiaobao.xyz/Article/details/gihafrueh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxklkguxh.sHtML

[P04] 求长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiiaaaca.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fanxiaobao.xyz/Article/details/gghhkwfgt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsivwwjf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboehzwhf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnvuquxz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/grslgtide.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fanxiaobao.xyz/Article/details/grhdumnzn.sHtML

Ruby: x.length;  x.size
来源：http://blog.fanxiaobao.xyz/Article/details/gqxxwqoaa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/guhcfofjl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fanxiaobao.xyz/Article/details/guecxjatb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fanxiaobao.xyz/Article/details/ghswlxoxs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gqqvqnzwh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fanxiaobao.xyz/Article/details/grmtyfbmq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrmpnrqn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfdiircl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glimfopmq.sHtML

Ruby: a == b
来源：http://mobile.fanxiaobao.xyz/Article/details/gzayiqrsf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/gaawufkag.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fanxiaobao.xyz/Article/details/ghteqnmax.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fanxiaobao.xyz/Article/details/glwkvrbxy.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmuaseoc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfupjvfio.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmqyedfy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gttcuobvw.sHtML

Go:   if x == nil {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzilhdgkr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzjlbsgo.sHtML

C#:   if (x is null) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnbebhqn.sHtML

[P07] 防抖与节流
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpvzvbht.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfbaggqg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gszkmrwxl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnqjgtfy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaxgucyy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvsnzlfx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fanxiaobao.xyz/Article/details/glldxubqs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gtqaptkxv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fanxiaobao.xyz/Article/details/gsxkjmyjz.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmnzjkfa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjykocyq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsamsqzfg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fanxiaobao.xyz/Article/details/gztyinovb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeptxhze.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvztixvun.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fanxiaobao.xyz/Article/details/glajilwfx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fanxiaobao.xyz/Article/details/gozyaekmm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fanxiaobao.xyz/Article/details/golghistz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfitcpgi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girbuxlup.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvoowoef.sHtML

[Q01] 创建表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxcwsyyd.sHtML

CREATE TABLE users (
来源：http://baike.fanxiaobao.xyz/Article/details/gynyfkzhi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gdnrxkpuh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fanxiaobao.xyz/Article/details/gbqpffemb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfduinjd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fanxiaobao.xyz/Article/details/gewuoszuq.sHtML

);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbgkhtow.sHtML

[Q02] 创建带外键的表
来源：http://wap.fanxiaobao.xyz/Article/details/gdjrpnlfp.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/gukvzpzkv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjdxlxhy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxbqwwky.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fanxiaobao.xyz/Article/details/gvwxdhyyf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtgsdvy.sHtML

);
来源：http://read.share.fanxiaobao.xyz/Article/details/gitvmhmtt.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/glyjpzeru.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gnkkdomgj.sHtML

[Q04] 修改列类型
来源：http://blog.fanxiaobao.xyz/Article/details/giubgkusr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/glnlgykpr.sHtML

[Q05] 重命名列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmslsptaz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvfgohna.sHtML

[Q06] 删除列
来源：http://wap.fanxiaobao.xyz/Article/details/gmxrjobik.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gcfkvrxno.sHtML

[Q07] 删除表
来源：http://3g.fanxiaobao.xyz/Article/details/gxmzusjtt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiwvwquv.sHtML

[Q08] 创建普通索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gigqqbhyo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebtckqtq.sHtML

[Q09] 创建唯一索引
来源：http://blog.fanxiaobao.xyz/Article/details/ggrawxvmy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjtrczgm.sHtML

[Q10] 插入单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gumvqhskc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gepmtxzzm.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuldbsdx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fanxiaobao.xyz/Article/details/ggompmyxg.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gjuppwyzo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fanxiaobao.xyz/Article/details/gpafhxnqi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/gpoxynpub.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/ghueftxvb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gahykvtvb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fanxiaobao.xyz/Article/details/gukebbazc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrxruwkq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gijtwrhbt.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdftvyqi.sHtML

SELECT * FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmvlihvwo.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgrnjzgf.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/golrhanxm.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gzslgzlka.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcajbhdfw.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gfktvxasp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtjjpncz.sHtML

[Q19] 范围查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaxpyzzu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmxxhdcy.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaumeflzy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkgvjtlv.sHtML

[Q21] 空值判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gygjkolvr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfgmklyo.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gwrssxfqu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgvzurfk.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gllsyxlvj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gxiubmfqw.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbuvmfwc.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gngsmmtri.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjmevaqx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/glewtqczk.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdwjiokq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzspoieon.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gybhgwyou.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsvcxpzv.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gdirhvdhj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/grrdesfiv.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/goamvvhab.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopqmyymv.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gnheetcgh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugiftdpy.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzirlwox.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gdifkwpas.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjasevxhg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gahxmlyua.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gscnvabpt.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvznwpgw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gvlzneazt.sHtML

[Q34] 每组取第一条
来源：http://m.share.fanxiaobao.xyz/Article/details/gboyhksul.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/ggghkpfwr.sHtML


<!-- 参考信息 -->