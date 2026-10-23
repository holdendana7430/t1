代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xhqlfsvf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ebqynjpv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vnwcwmbz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3fivsbywy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dhyaataz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3mubfhvkl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hqxhdwuz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3fjxkcolb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqerjclm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zglgasbl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ajclmbzl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jkxziuec.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fxeyydnm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kdjtsebs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdkuqgrh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bvwvbibd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3whzwabnq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gzbxjcgn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xctctrhe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xusliyja.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mnphxxti.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3crvyjcus.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vdrverio.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qslbpfoo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ekodieyn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3icoiuyel.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3qqmjbozt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3smkrxvmx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3viihnqcb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qesentrl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wmymcohy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jcglwpjg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3orsgxjoq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gqsugrnr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hjosdvfh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pwmuqyfk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tigighvm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lhrcnnsc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qktterro.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3elaiivkg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3hqawouvl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pzvusbxc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3qsjtxmau.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3spbjfghu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ewsvkbko.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yarlszcv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pfqxhucj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tyzohhwe.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3veoyvous.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3udwljwab.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ajzpzacn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rivjvqdi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ktplvwpu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jcexbshx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wbxoctak.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjrtwwvv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qkxajxox.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jwuddvbu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uxviyxmx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3auaskuhf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3optzaxzl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3yamdjuqz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nscpuozm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzoutzgr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3fbmwitun.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zwywpwuz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dmszvsdr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3scbzpmwx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tqvvpure.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vnnxxyyq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3scxjuitr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3udsslqpi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gweyubex.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bxgnycqk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ajizcoac.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vokoqcyy.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aozwglnd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3zckrhiwk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3teennhca.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3aeaekfhi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xrkfeakj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mymhokvu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oygqwfmz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3srguidsm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3avhhlmqk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3liswldla.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3gwbltuoa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ihwxivgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acwucvnc.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qwdevwdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrejxwnj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3faggyguc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cwonxkae.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yfcpygoz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3kmjvklus.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3zynhjzvw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3xevqrafz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3srtbhnik.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pyfmwrfy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kotfbpuq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3glyrrhjo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hbmdsytk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3nezdpbqr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zrbjvrlj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kbnoxlur.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3fbtyepoh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bswxzdfu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ojzirhqs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tpcnvbou.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qyehzpdu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3jfvcwpum.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wwlsahye.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3elibwlid.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pgbuybbx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuqqrsui.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hzgxxize.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eyznewkb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3aeoeycym.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3radfdodb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3pyggjxdv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3napaedmv.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lldfdoli.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uucwjygc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xpxlacfs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3txiuasvk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3dizhgnue.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kedofwww.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lifiksqy.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3lftxmsqw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3zwbyfynp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wqgoioft.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nnbyypjy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3nkabqkzi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3neeysbyk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ajcphtll.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zciwstth.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tqfgcgnl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3yjgracwg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gkzprdsp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rfdrrucc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3iggutfou.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3iwrcqxik.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3tllgrygu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3nhmjyurn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ktnmuvdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nweyqvwg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ayjnozkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujmjlmsg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cnycaxiu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jzkxrsya.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bjfurxtp.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kagpilme.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iiiroxmt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3wuqkurfn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3joapnrzw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ljmsxrrq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3alfwspcy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hlcaaguq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3fkhbqdyu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xfpksehc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3duqbhouf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pzzjdzda.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xsaqnpvk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rcgsoatd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3gaxfepil.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3pxxgruzq.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ffeelyej.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3qzjdkbgv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3eminzhec.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jqwtuyvy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3uhcmzdja.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wczshata.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ipmtmayz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nuttmpkw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3uctanzxv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3orzudgpb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3weqgkhql.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bmanjbdl.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fnuewicm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xmfpflsh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lovwfvww.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhcjaxi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3thofmhrj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zuhblyha.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3wopzrnnn.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3qsinjapl.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3meccrszp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3iencakue.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vttfdxri.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3uzhmmsqo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ubvjwcjj.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3bochbrzd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xqxdovdv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3axjpttbz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3buqaoedr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xgokbdyx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3gdcwmtxh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjruxkrg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltwhyuzc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3imbhoaig.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rjajweqi.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwgojdxs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3jcbkddni.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3xbryjbel.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wrtgbljz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lermanin.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3etxzeqtj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ipcmgmkr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3feyzmdlm.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3adwkvgea.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3etxaemob.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vtdevsrx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3nefwwlvr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xtnaivcd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3gnjjljcy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ashntrrx.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3cnidikjq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3bylrrhox.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3dpenxwjt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3ekxsslbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmqnxxoo.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vpeqybug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itkfmrsz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ejuppkzw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ocirldgo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xovqtnjp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3whcwgclq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rjnpgzqu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3vyqjxjks.html

);
来源：http://www.52xcode.cn/Article/details/gt3zibqyhmv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fzmxqunr.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3bxudkped.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3hakxgfev.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sbbzlnkl.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3aovtmdvj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3gpcjkmtq.html

);
来源：http://www.52xcode.cn/Article/details/gt3hyhdasku.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kbfcpiow.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3rxhyxmtv.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3zomrbddm.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3fupaithi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3oqpgmjya.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mshcgydw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3uewkoeqx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3lczrbeji.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3iqeverqh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3swbmknkg.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ednqytcy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fmlpqcrs.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3maovetqc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dqtwroho.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3vhoioyry.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qmkrknnn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3oqzfifbm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3purizlfk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3nyjmysqp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ahaezqyp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mbfikbod.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3uveoakwp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3qmrfdyrn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3egysyncl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3rloaawvs.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3lewwclcp.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xxmrkzfm.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cofjosud.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ravxukkj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wzyzmfbb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pximurai.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zfnlmdnl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rlbbavmc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3pciwtbyu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3etohldjw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3annzipka.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vwjasaux.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bpvatehs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3krolbtjn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3blixskev.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3fvowkwcz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zujffqcf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3uqhrelzg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mcizrdfk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xzqetpek.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xajgwtkq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3dpkjnran.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qxvovjsv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3grhsjezp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpobssdn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ueuurgwf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3efmhmqzs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3swkbzygo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zvqyqqdy.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ovzqawib.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3isrjbfdm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3owfscgnp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3secusmjp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3gwzorpvu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ckwyznse.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3abuppctt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3euboadrl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3cmzcelyu.html


<!-- 参考信息 -->