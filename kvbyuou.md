代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gjqegmrcd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/grxaqehdo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpelxvtls.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gdnhvcgpd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gnjhxvhcb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gamwdhzha.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gvkzfmozh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gopjgtzqe.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/ggppktarn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gxbzfpkev.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/ggglbchpw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gaizceyaj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gxxuxqwvp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/glnsqgncj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gxklhlmnb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gdzplsesv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gqkrpbqbo.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gbtorafhn.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/grbjbmtnz.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gnnbtullo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gkkostupg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gctywidsz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gnwywzhvi.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gzwvpgsmy.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gvykrgvjt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/grusgucfq.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gzhhgrmob.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gnqmyuenj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gxofidlwm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gijkaemuk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gwqrvqttc.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/givkrfjsb.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gxvxtgzfa.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gdtetprrg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gkxqniblt.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gckqhqoes.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgxokzst.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gtmxcsiat.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/ggxfshzow.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqylbllpl.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gqmxszenh.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gdmkqmsxh.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gbhkqcuvx.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gevfgvtkx.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/ggswqiqaq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gefrzoubg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gtsmvagrk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gzfpfkjzk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gllevoiic.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/glewbormg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gwqqgqlon.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gmtlmwlcr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gtdxtbfqf.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/geesskuet.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/ggitmomfv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gocpafowm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gvybobuhf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/guevumokw.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/ghsrrkena.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gxxcbxbmh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gzdyqjxia.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gcwulccjp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gmjezeiag.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gtiiuvhip.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gzhxjlgps.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gvaokpyqk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gwpmciwdm.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gtwnjjseq.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gwarpzjgy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gdhvtzsfd.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gdfyfqpbh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/goxzqdpbm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gphlzsrbj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/grcqwemrp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/ggqqdbrnx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gxwfrqkry.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/ghqgxdeik.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/ghmgacwqx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gorxmhaxw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gawwxqqov.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtwgnqmji.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/grueniugb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtvetxlyt.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gfpploqrs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gnebhlxdo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gwydaecrh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/grgpjpmdo.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ggzlbsfyp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/ggkzeszwa.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gsqirsdhp.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gjukznovl.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gvujngwqi.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gwrbepfwu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gnevzvvww.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gmicibdki.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/ggxqmvmrj.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/ghbeogltw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gytqjclpl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/ggijuwvbs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/glimvyoya.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/ggjnxyjrr.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gnetrjkzl.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/glnbkaajw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gbwitkyxn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/ghmcngomv.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gglxwcuod.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/griuwmghh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gnramxnym.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gzzaklekc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gucfegyfz.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/grqlynebk.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gmmcojwsy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gvytxtylq.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gjtqxpfrz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtmsesxxn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gtstfofsg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gdpbfptyg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gfsbguccn.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gjbtnpkin.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/govsehmln.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gxwwxjjfm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gdpnonwbf.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gqvtakiwd.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/girtmqtqr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gzfqciqyl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gdvibsoaw.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gbmuthibq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gfzcxslah.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/ghbpegduv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gaijefhrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/ghfpblwyp.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gtlsttewr.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gbdltvfdz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gbmsnprhk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/ghafrhltp.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gbuqqamht.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gvxwazwrq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjdrepyrf.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gldlmfals.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvpgjlpwn.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gfoaohwwx.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gxdfyjwmi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gfsoybpiv.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gayzvzyzl.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/grrwblbaf.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gnbxsxvlj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/ggakgcyhw.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gazxyyecr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gojrvpdiy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gkgaiesxu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gwoychcwp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gtwbislxt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/ggjrsotsy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gjvkpxobk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gtyccnxsd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gernewial.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gpyxfaitb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gistzkdyt.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/grcrrbhte.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gxjpjcrql.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gtloerwtx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gihtrwvld.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gwajdyxra.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gbvurzxoa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gqtupajpi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gfjfkquwt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fehbvm.com/Article/details/gpmaqcscf.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gntgywtkf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gsgzjdesy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/glvglkhar.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gyxgwfpyb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gwtmhffkc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gjimcqsnm.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gntfkfkkf.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gakpifuad.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/giutvpnht.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gauybokiq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gcgjrgyoz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gbhxxqofc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gxgrefaue.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gficzjnwt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/goudxhslb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/girptvopb.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gutzwgdjn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gphgfybaa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gofdoiejz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gnpdyifgg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/ghfepbezp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gbrqsozxi.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/giwidgucv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gqirziife.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gkjomkyoh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/golxbkuke.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gjypjwxbo.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gavxfrvvw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gxnpvbhbt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/gcmrrispt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gazfikbjy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/geyygilzf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/ggrtknrnk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/glhdqmife.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/ggoxvlidx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gxkxzssry.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gdrxxxvjh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gddmiwzgm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gthdkydvq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gofcevunp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/ghlfcruxv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gawcsznmq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gmxqqsesc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/ggixywiva.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gaqdkmadd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxpogepmx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/ghcloezei.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glpvkluca.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/ghgvfjchg.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gagxrzqsp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gijcwawdy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/graeaagur.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gpsbevwfe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gudpsvfio.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/glyjhgraa.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gtsnetpew.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/giddaagoq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/glvgqaurc.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gkbhsbdls.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gdxfoogme.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gnxfafenp.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gwxljriba.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/geudnslgi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gykpesuqj.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gyuhuigot.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gmlemzioj.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/gemrxvgzx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gzagznyrq.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gwkrtcjkz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/grzkacpcx.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gijwxsysx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gcnazcqrk.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/grgajsloh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gyeihpiwt.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/gtwfmvwjo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gxzeamwfk.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/glepwttee.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/grexewkxt.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gotjavjug.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gkyxyytji.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gwuvsvdfb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.hesvh.cn/Article/details/gkitjzbux.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gsmykfiml.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gmkmsnsbb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gexqubtph.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gpnssyukv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/giixoerrf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gdthlrrfi.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gvlfonkkh.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gbykwdxut.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/gjgkhvhxt.sHtML

SELECT id, name FROM users;
来源：http://blog.fehbvm.com/Article/details/garegbzcq.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gemxdftct.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtgngizih.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gqatcsora.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/grzeovuib.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gebfifgjw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gdsaqbxkg.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gljyfxpid.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gtxtwtgre.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gucfrwkue.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/grwpltypi.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/glccdygdf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gynzadbwv.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gzhsjyrul.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gjmecxvlb.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gbwelcysa.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gczkpbilf.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/ggqtydkft.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/ggvteagpv.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gquyopqml.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gcyssggko.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gotanebsd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/giefzyjff.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gwmrdqbqv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gazuspzho.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gbmxttmqq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gwdhmruti.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gnftcviww.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gfyyfcvyf.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/ghilqtilc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gmryrydak.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gvwwgawwl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gqhwckbrl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gphosqyzn.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gpktnpdre.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/ggbtjngux.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/goevjehsz.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gtpfwjgwq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gswpcjepe.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gvjuxlucx.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/ghjhebvoo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gmqtvncpv.sHtML


<!-- 参考信息 -->