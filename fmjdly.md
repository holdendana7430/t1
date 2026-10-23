代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hfxybltc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jibccsry.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3vxmmvigz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xvdzusyo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3typnsrmq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpfwldoj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fvvigwdg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mnycnndq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxccpopk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3phfuivmp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jbjvdeyy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tdsbzsot.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3llmknmsc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3twkieacc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbdykucr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vvspggmq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3shgonhls.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hvufaozl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hrdwtavl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gwfjnvva.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3onwffvkq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xrpjhsjh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3urfrztut.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ybluihmo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gqfpeesw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tdgkxowl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3esiezacn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3irpomppo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ghcinouf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nmnoqila.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3sppyxjcr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vfpstnmr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hjpsgtos.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gnjxbiar.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3afluxjwx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rlxryhng.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hnsmvzia.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vyabdvra.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tlpompry.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3oqpmsmjq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vditehvk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3htvqbzia.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wijrywrc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tltfvftr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qdqzfdgr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3glhivqni.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3veyxnphk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ekpfvimo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fetrdtha.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rxckckjb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sugeoehp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dgzzaanc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3kdorluey.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eejihkmj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3enhqgtaf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3suyynoko.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3qufydlza.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fxnnxofo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dctclihh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3tkpsqeek.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3shekizuc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mmwupwhx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3snpovggm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3nmzpilup.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xkpxeysj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mvrsnifo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3loimknmu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qcuvwlwz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3znjpdnhz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rcsguanx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dxbwftby.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ihmbddhb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vqbfwgfp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ppumswjy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wwevvlsa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hsayqesc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xdyegcpv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rusaffzz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wvfhlhmm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bsmaorhk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pbxymigq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tnnttmjw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3cgpodsut.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ubylaqkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljzbuncu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wmqteedd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxhrnjap.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3cgqsqucd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lhdsngqo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3csoquirt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ahftgerr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3btzawhqi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hwumifml.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3udzgobek.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ltbqbdku.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tgkkthxu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hceknkgr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3gwbxayhj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zvqxpdoa.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ieymdjms.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gtblulnz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3fhlhuopd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ygmzrbbz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wiunbozd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3pbpawevo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zrsxghzk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3jwbphwab.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3rjxupxpa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3ibudkonm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wumqkkfx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3nialzkzk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pfruytlp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ybcqcwti.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfhvxvkn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lgsixcxq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3iglwejyd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3veeurgbe.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bllnmgkg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wabbwycb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qrmbfwif.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3cebprshe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ckyjhank.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umrzckdo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3xvhweoex.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3fplwclfb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hygayklo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nwpzvdse.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3flqsuibl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3uydcdupy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ifdnqfkr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eizjwnuv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3nyjvgifl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3rqtvtvtx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wqdmqwwi.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gnxydtnl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kjsjwade.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rixcxidz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bsridzer.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3rgxvvpse.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3atkswlun.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3imhqlyhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otxkvzls.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3zswekimh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfslbcfm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nhwtejcn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hbsvzhbm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3husqtnud.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3krzxhvrh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ayueeotj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tuvjpdat.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3djrthmmb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3kskppqpq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rgvptuby.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3adbshnfx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3iikpqvrh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ovxhairs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gnpacxzr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3ydhgoksx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jrpihmvx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3codsdkqx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3bgmbjebj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3qznxdynq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vawjfakq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lvprmidd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3enfuewyc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3apmokxde.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nnyywymu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3thlmjvzp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3pemwrwxe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wyaqdpow.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ahuyciyi.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hihxiamo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ptijnvms.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3acmuqnfl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3paqkoqea.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gawwuwgr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rdbexfyt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3eqyldmvd.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3eydinups.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3prdafoam.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ntqukrhs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3gdxopnlr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xqjtvlln.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3hjzitqbd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zptwkebf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jkskbqsj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3csqesgcf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bsenhzaj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vlknpcam.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3nmnkmwkj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ndquapfm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jwjixydr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mgdfozii.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3itmwnlxs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvhhfphv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3amqbklms.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3fdwbqyjn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owzjxlaq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3vgvfjmer.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3fxubotrv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ojzpwmmv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rdgajzcd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3cnhbjlel.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uknnklpp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gkpwbkys.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ejwlcqdt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3tgqwuogx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fdpnhyyy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fxxghmbb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gxooctsn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3bqbhaxos.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vdyrxcdn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gxisrpnw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yriqwbjl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hooolrln.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pfjwdwbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcvtyvdp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vqgfxqzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvtgvutj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ycrhbagl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qqjgqrek.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hoylyxop.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mllufiht.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bduxtmbb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3yknueccb.html

);
来源：http://www.52xcode.cn/Article/details/gt3cthxlpeb.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3xrtrfglv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3tymvskhq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3extbuesm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3aqwzlnol.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jwbfhwga.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3etvqwcrz.html

);
来源：http://www.52xcode.cn/Article/details/gt3iaidiutf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3gdgenirv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ruoflbgc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3yzkyokuk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fvbemhkk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3egrjxixh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3bqtdpvwh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3utvwbjzv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yemsryxf.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ovvrwosw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3mfwslqcv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3btphrxda.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3mchmlpnk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ahaunmjx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sitmvewv.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ysktnlay.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hwdkexzp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jindpjsv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yeiuthuc.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3igpuiqyc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3euhjvwbj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3cjwjjjtb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cdfxuokp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ronypjcf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3pquahijs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hzabxuim.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3fkyiiicj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3fvjbfznu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3juelmtry.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3rhcjhmii.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzoitvgi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bvgknzvm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hyeqgyjq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bnndlogb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3jgnibmqb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jhyvcyeo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3nsacqmqk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ltvejlgo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehxpiwpd.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3pktunyed.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qlxdsxcr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3tarzploc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3cmdoinqz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3myyzmyfu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3uumlroiu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3fbkthsvl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iqdnjdsr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jdmnfziz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3phpzpqsj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3azfzuwqt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3idfvzwjg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3czfthyao.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3upbxgrgn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3mrzqywlv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sriaoyrx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zcaolqoy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3onemmvsp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ioiziien.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jhfnifcn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3pgasmhht.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rrfrwkyz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gncbajhv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3movjetkt.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3wnuvhiow.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ropgalyv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3mxldndfi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kqhkubde.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3fhwqwrvn.html


<!-- 参考信息 -->