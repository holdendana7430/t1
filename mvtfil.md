代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uewffqwu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2cuwiexuf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2usgomwlx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pizmrxfe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2izwrnghw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfchibdd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2meacstap.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2enbigyrj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jhvcndif.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2opdnflfd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsbhzzkm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zfyibdhx.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2edlebeym.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wvkbibnp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fdcfiios.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcthwnwr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzvborvr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2grynddxd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2aytbdixa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dykexgjh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2bbxwbcev.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zxnjhhid.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hariodhf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjkiscsr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yuwghrbt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jwgzfhbb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gbzueygn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rqijvlme.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wehgspjd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bxjxpssu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rvcqycmb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2etnzkdpt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2isefbjsf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2poffewbd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2plziooil.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ciurvtkl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2cvigcrgr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lmtxsstq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wlyyxcnz.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ilqmgyjd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pbqjhuhi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wklfitsb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pjenbyat.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fexdypjs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wgbrajrs.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rviezpyd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xigkqwww.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gpsynxmc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lavmwmvl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pgtiovjk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jjnczfie.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mvkftjjj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nitdxlwm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2azdazned.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mqhknyos.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nqczbqtn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2pdprcmkj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2zoruojtp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ufskress.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgmwtpta.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hgpydnrf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xhyfctdo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zrlsuixs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2maqupajf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hwhbojry.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hahfcvvd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cjsdozrq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2kzbqubaz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulwgtxkf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2axqffwjh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dqqudmcj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xxyayzjk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2esebzxll.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2urfzatft.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2itbndmcu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pwjghwga.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2avzmrmud.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vowuympa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gdmmgkgc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dlizuxgt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vixfimrb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jynscmzc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jbfthosy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zshkmcmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slhhiqxl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xlgrevzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phzkariv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2alsyptog.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ygasofpe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2kpqlzlhh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fcdlbtpz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wbnfsutf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gyzkhdne.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ngescoew.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2itlgxcim.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vzedaiyl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tjzqoprc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lxsvyvyo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rhnoadhm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xqttksje.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yjobaqol.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ymrzvkqs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2shhphryx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2yzwmwhii.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jcftbncv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2rlilmsmv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2clypnmcu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qugjmqco.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jidytidv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xddvtdqe.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2croxmavd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2pqfgfzmy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2odxquwuu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukylqskw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2imviaqjb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tfxsouzu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qndklbmp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaomkqpl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mplsqzqy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2muxpjmpy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tmmlumxf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kwaujosn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2diushpca.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2akzedyem.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fnvtlfdn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2liaenzit.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fpkqylgu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pxbnvshr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2jydmurva.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2foipesmt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2aovfjqrb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxpikske.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2sgbttnkj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2bxgembvp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ykymjpvd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bfmapsxz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gesgdfru.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ombhmtac.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2hqkfrywl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2erdhfdjp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xyqnltxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vntbvume.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2srljcfag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luncmrct.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cvuagpwh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2guhzmhvu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2xazurfaw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2asngsgau.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tztnuoil.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xofilwpg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2aksncdmg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bzlzokln.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lyllhnaz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2woqoxzvw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ubkkcrsi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2pibhdrha.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2iptshimj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ekhryxxf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ppdlxabo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2cajngpjl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2sraldgpg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tdkohpck.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dbfaadxj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2kvbqqpzr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rjlmtyit.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gyxqycss.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2kptfonhl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2yzzkwrjm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2kkzeuqgw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2itcczgcx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2grfzvjrn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pppokbki.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2uvqposmg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hpqqfpmi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2utwdbsom.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2repozrtj.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ujlmuzwo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lrabtrkw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lazziuuo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gjjnxsta.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2jbjjgaiz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2jtqcsnjc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2sxeeanmo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2oqkrhozu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xdwikort.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2kmgjdpzf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrfifiay.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2doawrpzz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2trubbcxj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2uxmyxxji.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2uaqdnynw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdxibsnr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vpcklihh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2jqrwrrkf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbdngxem.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vktmfrrw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hndagjhv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ilmuwche.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2eauqgbbb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rdpribki.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2edzfnrme.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vwvjrmkz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2igqkxneo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2nuqtmzgx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jaohshxx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2vutfaxrm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2naibwtzs.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2spevmtml.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2mqgvxpwl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2cfzcnedv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2vryrbmyb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmcyuxve.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2yghfpaqy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2oxjyptyf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2comjuusp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2rlalgwuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcwhursg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2rvgscznd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuismasp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xffhhzam.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wfogymjp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2iezgbsuf.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2eapacubs.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2odttykog.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2izbjotpk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tzpbslwj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2yyfbxfup.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cebedeao.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kwgjefqv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dkqomwkk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2suvrdpdq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2virgujby.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vkjethgd.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2cznyokcj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xzxierxo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qpshykez.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jivptgys.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xwswbawm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2yvambfwy.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2spokrmii.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kbahfvct.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2yvabgkqw.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nfuaeqbx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2gsjpuxhn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nwtfhyze.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2oycmngkc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wgetezep.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2nffjmvuy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sxhbpdts.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2vfgdocnb.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2orrucjxv.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2wiimarix.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2pthqnivp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2jxlhcdys.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ojjliahx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qyllqtqc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lzmaauof.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2valhridy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2vijiznzn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2xpgmftlk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wxhkuddt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xgkjsfol.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ttlxrnvf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2fiqpgtqf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2miskjrju.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ukiffzxk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fcwpvglu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zqsclvxp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2qocqiuvd.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hyxhutfa.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ukjvxrht.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dweagfto.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wnwfjphs.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bsfpvuce.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2smjeiods.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ujzvxlan.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2omvmdzlt.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gsyytzhq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bizfkebu.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kylkmlaq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zuioqkzz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kmybgetn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzawcaxh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2sjzyinqj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2diwtkoai.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2oxculvep.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xyhwoolx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vietxwcn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qcowvtve.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2mnenpqvg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wjtsbzgm.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vojahpzd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2gjcrzsqr.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tieuanhg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hkaegepd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2znscbyak.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2tlabyhgg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2gzzrmhpy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2dnxirpxy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2efscmlbq.html


<!-- 参考信息 -->