代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tmvbwpux.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tqoauoez.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uhcruibn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nbtfcbfm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pxnzmdty.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wpfqzqva.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rzkoehtx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2oshajofh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rghxrrcr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2voituqxy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qambfjoe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ulhyxosz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xwyrqlsf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2voxxgrjo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2igugaqom.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vgadlkji.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2weugbreg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yfwwhhxo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2pduokbdg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkccqyfg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vquqskgx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2eqmqhmbf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2pupisrxo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mmbobebd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2knceicux.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mdgyawlq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ldiaxbdl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nvbmcmgc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2syoncjzh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kdeqpmvw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2iocxehrc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ppwghnhc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ltvtsdag.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uomdibuq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2rilhuwhy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jlyjcchf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2zvlfwwyo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2levevskn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jcbhggjr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gsifldgx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2iagvhjof.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2igvzfvhg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wsizcndd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2oftexwcx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rexbwfuf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lzcwdups.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2havqrmhe.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lfxmyrqu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zvstjxfu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xcxxtpxv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pyaomncs.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mgzitzqf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sjbqzsih.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oaatoefu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xfeclzex.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fbaaerwa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vdrsmjpn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wqcmrruz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pniimvpw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zmxybwig.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2faagbvpw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2dckrxtqh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lnadzyeo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ihmbnjuo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fbxyqdif.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2jnxaeroc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwosnrnn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2npudqedr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tcziepib.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxbztfgp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xgsozpcv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2wvhldbfg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nztzzfvi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2psqmwgjp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2etgjaxut.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dlkzbakg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vedwwwaf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2lrmezhzx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ozzjompc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2tztjkqhk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eximyzgi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2alfpyhzn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hldwbazp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xrhpxwwn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2skzcpxdp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rxgadwjt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ecngawsu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2deaidcuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjddkpxx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jzmkhyal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kokpfdoh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2brrmmdja.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wnxwdfkh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2bewfxelv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2npnwwxcn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2erscgtyp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vfdgvoua.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ikwydiwe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2zfmpvtmd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rloqeijh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ydcjedvq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2zjmyabcj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hbyvldpz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gqjkqqeg.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uidsbbnj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dopzppzv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2sluqzdxu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xftevuaq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2zfixoriw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wyhfeljh.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2itrbhhfd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jsipdchy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2nzacsqxy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ftsscyft.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2djgoaytd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wugukvbs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2lsccswxv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dccajgak.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jpgcejoe.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2jgwedfdd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2hloaiwmv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xjwfnbdo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekkpfkck.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2euxoftok.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2bzobcolk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ekozthon.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2buwcokth.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2sehgskny.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zgwzkqxj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2uyctaxqd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bqrsvpxj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kglzhfvp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mlksznqj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bkeorlyr.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbhtxfh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2cvskpvur.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qomezkih.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2arnphewu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zjdkhukz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kbwuyvkv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qvrslcdn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2athvesdc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ryjgoicp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lfpuxfog.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2bzktogzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umlpgehl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ayiqgzvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idslojbs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mmtxmwvn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wyzvvhxi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hclhgaja.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xizqiyfj.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2khpyetrw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2sxesbiuq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wysezdwl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2oxhqklnn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2mgrltnwh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2sozzmkos.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2hrcngqlo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ccufwsnz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2klobhcpv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2wqxzxxge.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nwyccyic.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2aevgjses.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vtabajug.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vvfozxpl.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2bhnvhbbk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2vvxaqeiy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2zrwvujvm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wbwhyqax.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dlifnaay.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vwxrvhno.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rpjjfyps.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ggavssab.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2moriygta.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2twdmlsaa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2tuwhticy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pthxdtzf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uyyocwer.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wrxhedqo.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2daybckco.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2yppntqmh.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lkhosxwt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2smkzxpiq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rubgnrjh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2iiagycql.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2rdzvfmfi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lqiqjnat.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bxyicghw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2yzbsvdar.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rvzixsqp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kdawgrhp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2kiecrtqo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2zxukmoaf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2lfpeavkh.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbrmuuyw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2flkightx.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfiqhriy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhsyxpse.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipeludil.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2cumfzefb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2dhlmhzaj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2snwzndko.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2zmaoimig.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2lbmdlxzc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ccqgvuzk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iosnbooe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2hgpovzee.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ezstozby.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2suegolei.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2zotwdeku.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2taxzbuxd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jqdzitcv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vefxcvfq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ejkrtvep.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ypwimqyr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2tgnpeaph.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2pnkrqsvn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2rhifgzih.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dsykqfxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajnyoxgm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ywcjhmxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omybyzgl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qvbhjisi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2pirvjtge.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tzjvkvkv.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ygpiliig.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2syrpsmoz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jxdmgxol.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ddvsqkjw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2bonbersl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2vapjfxnw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bdvhympr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2lquhtzmg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2azbnooex.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2mmvzoepm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ebxhwpeq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2kxszcwbv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ljflahmi.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2tpvevvnm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2pfipgunz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2obljegpk.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2vykkzmkf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2sosklmvo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mflqqzad.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2daazpeqg.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vfqbdptx.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2gwzxteor.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2rsuczbpi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2mwczhauc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2umymeljh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ylhymkhb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2varfmosr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2rcmwufqj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zemwxeuo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vmhakbwi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lgefnsgw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ftvgivmi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2fbqwaiwc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dihmrnxt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2aenlswpm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xlzrzuxy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2snvrteub.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2dfezomjr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oqhchlhm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gcbhyfcd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fkayplgs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2monxpyrz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kccymshb.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gkwybfft.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2yohtsqug.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2pksziynh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zlygxgea.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qwbiyiuw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ssympfcq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2dgnjqbxr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2spftmlsb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2idxurnyg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wiqyrela.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ighjecsy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ghhflmok.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dvupnqzk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ghfcfubd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hfzatgve.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2snaeaejc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ehdhndpt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iopcwuld.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2anruzhae.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nzxvmehq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2aipigmhc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lswvxodz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2twsmkknc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdljsrpg.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2nnqmgjfb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2brzxastj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jmiycqqt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2nwflxmcn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tdsmiadw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nnevscdb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2xrncpiwv.html


<!-- 参考信息 -->