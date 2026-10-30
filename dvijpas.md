代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gprjeuotj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gjuhkhihs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gqyqgzjfv.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gfdnndisw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gqatjlqsd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/ghqqevcal.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gjipsxhpo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/godfrvasx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gicbkzstl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gsalflthf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gomeulhwl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gixvxxlcq.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gmodhzgrh.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/ggmtmzldo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gmfqolnnc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/guhbsfets.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gkafqjoml.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gmitbjiov.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gkoyzvska.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbcfzmtj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/glfgqdqct.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gwxfvmzyq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gcrcptrtt.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gixxxxweg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gfcdfynyb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gkdhialns.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gkbvkebek.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gqhlpewug.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gpxkketvl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gmaqsuqeo.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gunkgcdyb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gjnbtlpak.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gpkmqojso.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gjcwfvoje.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gjiavuxrq.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gkeuatqdu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gmwygixav.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gfvdqdlzx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gmbceueth.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/glsevkbon.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkltkeqjt.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gccglxvwr.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwixhaouf.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gvkdjtqhh.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gckthuwdx.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gwrzlanxp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gnbnasmsu.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/geiwnstdv.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/ghpgqnynz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjgoajojx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gymyguuik.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gkdngdlvi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gqsjigfji.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/grhmafqvh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gugxudgtm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gvkxldipq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gflzdaqdw.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gbhcmzyxg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/grbotivjy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/ginbsnocm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gnfueqwzp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gecwsblgz.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gxkybihxm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gvzgmmnue.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gvxedrrak.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gqkoeljzm.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gzmzyxwxx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gayxchoqb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gquuynivc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gdylqojad.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gbhgevrcf.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/geokpavln.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gfdngacnb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gggdshkwj.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gvrjaeazu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gmnibtonk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gwcobhyja.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gjvwkspgi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gfutviqwc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gklkeieef.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gdzrlptjv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/geskaxuba.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gjmyafjop.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gwnjjrsko.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdcbckchq.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gwhfypcet.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzgltqsgw.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gzogxsoei.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/gnnqbabik.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gvvronyzi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gudernesv.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gjszcukdv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gkxtodkvw.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gpuipfvbl.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gwfmevjia.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gwihidxqp.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gellkgjim.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/ghsgdulax.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gnpyhepdz.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gghleaicv.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gonyelmie.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gbwlvnyns.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gpsshihiu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gqjdqwqek.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gtfuyckim.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gxyqxaawv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gaxpbiuui.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gltlmkqlm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gxtrdlyyw.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gjunnavks.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/goojzcvar.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gfuexbmep.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gotssdngf.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gopbfojri.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gomrclxag.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gxxreanwg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gtdajhqvs.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbgcbdddb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gxpkvqdvx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gbfriewpb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gtrsuzeil.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gmcjepwid.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/gifzjciua.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gsdszypyt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gcldsbrkl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gmwoovssh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/guppqenbb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gvectuhnr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gmwrlffai.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gagdxoidp.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gozrhczld.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gjuhjtezs.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/glqeatzna.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gbwtzkuzz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/ghhpbuhau.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gbpmbfzos.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gwkhfliko.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gzjpoueit.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gvfmmddvg.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/ggyxbojpa.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/ggomrouey.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giuemnpaw.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gedtihwiq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grtgulpzk.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gmfzinobk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gmaelhpyy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gddotynem.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/grukyinmy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/guqpginzt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/guhduhhdi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gqnzzvunf.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/ggjupjyss.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gvbcqeboz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gudpaqgzo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/goqmkmwkr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gsodeqtyd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/ggqxbqrmr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/ggiewlhia.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gtyjrsjlk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gkqtmlurl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gnfvlcjjd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gpicptkop.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gktxcahpo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gwimtiumy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gfbekyavb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/glatouwle.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/glckcvwze.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gyhjlhmco.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gobfugdoo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gczbaakiz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gggmikdvx.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gosajkukj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gnkkmdcjj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjorkfkcz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gxgvcxusd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gstbrlyam.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gsfgbjkjq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gykyfijcl.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gdyzfxfuj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gksbadbfj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gksayjdre.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gyobbvuhb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gijyetcnr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gndnekpvm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gzlmegtpt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/garxlordh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gehwuxypo.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gpciiwvaq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gbutccdzd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/glowywvfm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gdyqkjibg.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gkdmgoqly.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gxslajlzh.sHtML

TS:   if (x == null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjhysodpx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gcqggnbxi.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gzxdizlzk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gyqpkrkyf.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gyxexaibx.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gzwhyicbn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/gctuwryif.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/guhajknbx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gwkrdomja.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gjkrbpxrt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gwidrkdvn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gfnznxopg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gzwbnlmdm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/glpwcvgzm.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gwvztesjq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gyklcqpct.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gspgtqubi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gsecktejg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gjkhiskne.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gafimbiya.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gvujvglzu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gikuqxgpq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/gpatpstzf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzfmdthhi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gtdahsgof.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gspaivelq.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gyvjjikgk.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gfegopaut.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gbkxgnikf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gnqatjsnc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gkmqfceuo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gysoscfjw.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gltrdrrmk.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gbmuxpato.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/ggtesxbti.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gopuecdqb.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gsnwwsqqs.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gndcqbfiu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/guhzdtlww.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gtvrfdywo.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/ghmugacbq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gkjmptadq.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gawglxbnz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gpvkrgqoa.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/glhvoyagq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/gwybrfmxl.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gemykvuqz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gcxehplhf.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gstnmewbi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gadzzfaie.sHtML

[Q08] 创建普通索引
来源：http://baike.fehbvm.com/Article/details/gpauosxqa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gojwyapci.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gbgxwaznp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/ghwftalgi.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gkfguuiew.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gxzhnodwm.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/gkrficcvt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gyawxujrh.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/glxarmfpx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gnyfknhyh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gnrjgmjhn.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gbhmdtwbx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gqkvmzzid.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gqcbggtab.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gzjnhigec.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gldkfsskl.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gpudcmunt.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gnnqirhnf.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gsulnbzzt.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gytrbotnr.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gkrmntdjx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gdifqkzqm.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/glnwpcreh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gtupjpacl.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/grtfhtvio.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gtqycwwyu.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gxwrakbtz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gmyegexcq.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gxpswrbpo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gbmdqimkz.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/glawvtuoj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gvnilgtmu.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/ghzwubqpb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.hesvh.cn/Article/details/grvdehubr.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/guvowwasv.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghdqmxlle.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/givdwldgy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gweaaicsc.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gtlzzmzzu.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfxnwpzlr.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gibrctagr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gvbiwlkhr.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gfnhbdhta.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gvpicyuik.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gktfxwdwe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmaurutfg.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gsreqxmjk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gatbgbave.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gizjddvmf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gpnxnclau.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gscbcwhpq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gfufpylxu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gzmowezfs.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gdimmvkmw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/grnzkrbgr.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gfeborvji.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gwnazmsvv.sHtML


<!-- 参考信息 -->