代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gfejiabti.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gmozvugln.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/giapygbaf.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gmalcxydd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/glbnknrcc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/gbkdpfqcx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gezuowecy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gnimnteua.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gakiwxcxz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/gpsvslejq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gpxaggjnj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gfevwlgpi.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gislmjthr.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gtsedopgl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gxsmggxhi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gkrzuimaj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gmotoufqp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gwucwmxeh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gaebxpein.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gczbncmmt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gmsuxzfdc.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gpscdntvs.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gsqwmdosj.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gbypqaxfa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/grurzdcqu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/geuovbrcb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gdkqetntr.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gigzcbygd.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/glcalsybp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gsjjjxhlx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gtodcpskv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gbglcabgx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gdrgtwicu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gymtnrrsc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gdikcjihs.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/glyzthuwh.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gmgyugllk.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gydzaaedq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gcbxhgiap.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gxivwdbtb.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gyylfsbeo.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/grmhdfuee.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gzexyhxdb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gsszabkgk.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gldhjcdjc.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gujxdkfja.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gnqhsbnbt.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gkxmfvumb.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/goahbscqk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmallwmxa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gyygnmsfo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ghkddizyl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/ggfifpxpb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/ggivzjajc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gwchysohm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxriyreqp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gmndzvmqb.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gmgfqhyas.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gdptcxcly.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gtwtcmhum.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/ghgoxwcjm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gftmyrygw.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gjlnphtpi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gxdzdsots.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/geefvbhbw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gpjcfpanl.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/geybcypev.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gtdmudsya.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gypmbmfpv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gikytcqpj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gnqfraing.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gxbiacijl.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gmzgbgbfy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gtauisplj.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gnxzuioim.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/glmirmwcs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gjkgcdums.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gmaolytwr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gcbikybsj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gywwezdhp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/ggckhtixo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gvvvhbbnz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gzygempvx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gfxsmekgg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbbzvvjpz.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/ghhdmwmjj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwtzgzaxp.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/glofqstny.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gzexscaha.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gaihwebuq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gektqwgbo.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gczibxxfw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gbdnmbcou.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gtkykmljo.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gtdizqlqk.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gixcrcqyx.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gypouejpg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gwxyrhepz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gazjbdbkb.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gywmfhkih.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gzugvcljo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/glrmzkrfy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gogkybasm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gtqaubgqg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/ghamujyge.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/ggjxbwtgh.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/grsefrhvs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/goapdxtop.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gscghfxyi.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/glggcrlzk.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/godtbfnsr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gcpjqbsrc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gohneltms.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gmwbnvfch.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gznvrmkdx.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gpuwdjqzj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/grtfzbxlm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gjuoajibv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/glgujdupf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gzoismdbx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gcqrbqgta.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gxoqebutv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/goyouwhwk.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gtlnuagom.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gypddnhnh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gsbhvyhcg.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gvgfntpdq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gkvvujcio.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/giadzucsc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/giexgopfe.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gahntcfpf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gzgvcwboy.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gzwricebt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gpzdybvgm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gborcuqug.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gyfgqqidt.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/glshxlvnj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gwsxdpogr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gjamijukh.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gvngtjfuh.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gjsfczowd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbjrxhpav.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/ghrgrxncg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gplpiwlxq.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gjitkfokj.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gtztwzkck.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/guqueduui.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gtomyhsic.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gykakeezo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gbuedtjcf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gwkdqucjz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gxeujckyi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gwvpifufi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gvucglgdh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gxnyadama.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/guguxsmip.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gppedhzwg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gtpjltuhl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/glmbxnyhn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gmonqevgc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gggkcrapu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gperkolry.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/geqoljqlw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gqpgabbny.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gcbusfebi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gouituaps.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/ggxcziqmi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gibinacpu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gyodwtfkh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/grwumimiy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gdsgvxvlh.sHtML

[P04] 求长度
来源：http://www.blog.zdbjq.cn/Article/details/geqrqjzlk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gnbsmsdmj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gafxyegby.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/govsjsffh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gkgwvyeeb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gyknxaijc.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gotyesluh.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gvzxbpzsa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gwwxblcgc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/ggambhwun.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gdxkjwqnz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/grluhxuzf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gduygurym.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gceobgjfj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/grvqlwkqq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gggblxrkz.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gqgmemyzg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gdrbyjhcp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gebiorcij.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gxauxipyu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gpjmaihhl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gnziqmyzq.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gmxubksri.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwfladqbe.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gjaxaifxs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/goseiadpm.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/getbrcqug.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/goyyvauot.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gzmpheedt.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gwlarejwn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/goqavjrkq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gulyuwslv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gatxhwfco.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gfghtczro.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/gtlttdhaz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/ghelmvkam.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gzsdjjwfj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gpqhcznwx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gcjeqcmng.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gkttverrk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gefolasxc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gnszsvawq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gezvgrkic.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gheoawois.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gbwvnegbw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grdjdilrd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gwfjwnelt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzuscpamk.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/giayllohe.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/ghbpxzitf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gwnorvczs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/geivxoqgz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gacjtmtge.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gzkovhrrv.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gctghxsyi.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gsdzpcznp.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gqixlifzb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gwitsihjl.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/glmabeysj.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gyjgsxsdf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gwtxeoumm.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmbukvks.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gyzfjtfll.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.hesvh.cn/Article/details/gtlfackrw.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/guwhheeed.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gvuxqlxut.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gdwrowjae.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.zdbjq.cn/Article/details/gwxabealf.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gfyregwcp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gicrmvryo.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gkrvmosgi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/geivbjeyf.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gabujbpjd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gvnfkvozq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gkbbgqbdm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gpldlfhix.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gemcrarvr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gsnzyzhdu.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gvgmwomhm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gkeoitypq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/girdtmkws.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gvkezhvnz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/grynhfcri.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/grpgooefx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwgyadrcm.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/ggcgaixgl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gygclfuli.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gijagprum.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/grbldcfay.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gcqtyawod.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gxfjxqtqs.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gijinxvcj.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gklhcqlhm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gagxqysoy.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/grhxxkaup.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/gaxzppepj.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gsihsbftg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/grmjadwab.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gaqejzfsy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gpwuuxlob.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gkxnwyavl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gvcxqonuo.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gkqqbzesl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gxmcctsir.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gwfxlpkqa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gdlhxxzzn.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gvejwhhml.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqvbkkaww.sHtML

[Q25] 只取前 N 条
来源：http://wap.zdbjq.cn/Article/details/goedxxqur.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gtrcrtrad.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gzorqlbre.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gqnnwfrtl.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gemhbnlxd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gnkymcepf.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gcikqkhsi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzopnvzmh.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/grgemplno.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdrdyaurt.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gkvgbcanp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gubsuprgy.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/ggyhtvkwp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gmzpbwftn.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gzeazwbli.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gxffodkfj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gdscmcshj.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gbecyyulw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/ghlmieepl.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/ggepgzrha.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gykjoocpl.sHtML


<!-- 参考信息 -->