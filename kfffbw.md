代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bxwxghww.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3doxxmdtx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xmpmdkxy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3soznrivw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dtlnipym.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wckgmwft.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xsjraqcu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wheaezyj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3efqdtvrj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3hrxpszvw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3stxiufup.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cqgejdyz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jufjppal.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3rxctdwzx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vmulfsll.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mnjtdftb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3waftbrod.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3aulzitsq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vczwifzi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3szjkpvmu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3lnleahac.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tkkgrkin.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsshlfcx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfwqatfi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nvtoccen.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vnaitdtd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xbosjjyn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lqyurmsr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3yngkaqih.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3scjbyptd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ekiyjthn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tsdovcpw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pwoijzok.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3axjgtgcn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3enppjoun.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fpigqbkl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ygzpqipy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jxzdftfr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ioiixtwy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xebipyxz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hpxejyvh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mjjpkvba.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3mumhxvsd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3eoimzmop.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yiyoangi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hapixezq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rymbapgu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3oymhneus.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxzuwlvs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ojdjqysr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3krhupvhe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wdifqqoj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jkbmisbp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3melqcvqg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pbfetpld.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jgccnuak.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zcmpkixa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3czbmxpjo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gymiefsy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3alwimwbz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3frpnpkxx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mhjjnkwv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ubfimzgp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3asdkmjbi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bccirlvx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xxwwphcf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bqvspgbp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ftzwqkgi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jlxrirga.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3shqaixll.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3covkcyya.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uamwfrmb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tttcfstq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3btaylbwd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3etjakwcb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3exwjewjv.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3sexayzuk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wpkogqyo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fmfaroil.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3egnrfnkp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ugiluive.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uoihguld.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gwgqvuzt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3puvyugiz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3krdopylu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vnfoapkh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ngvhlwdu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hsuenxda.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jrjrevzr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3roawnuhm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rmbszafr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bhchnbju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pswrtnal.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3jzhbupyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbesfnij.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3leeubhcd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lmoplclr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rudemyko.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mitaysat.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vweiunry.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rchuggzg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bmxitkiu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3xkbjcyit.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3zobuqioq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3szqehrom.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qfqkvmqy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3alziwumf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3chunhjwa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3sutevugq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wxedhwpe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zguhdnfo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3kuidwpla.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qeuxjsbb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3anaaqwse.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3rjyfzojd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pdcmmpzi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3uyeuolsg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uwqdzwqm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mrdagpbu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3oybmjjjl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3fowshjft.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uutokuux.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ursoghhl.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gagoxidr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ggangnyq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3lcquthhy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dimvugjs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3actmkjbh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3hcufizyv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3oahidkmv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kaczqkzg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wtytzsni.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3euvxanid.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tfptzmwa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hkizcgfy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jvckpbnk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3biuwxpty.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ponksxek.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3utxsxwvg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mbishqjb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ngovuoey.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3orxegkah.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3kfsxzyhb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ippzfaly.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cezvbwra.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3wflkwiro.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3jwifsvlo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3eacpgsxa.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3tzmobefq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptoejdxu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3snzujihq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abqakutf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3bvhehlgt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3qdscoxsc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iabjxuhn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3moeuqusz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jqwtchxg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cnxtyavo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rfeubzbv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3trspstsv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mtbndmlr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3ngxngdpn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ejtcrtiz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jtzmuswx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3oqozqotg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3awdydzyn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rhcrhhms.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3clhgertm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ehfttvil.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vxisdney.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xrkdmogm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3svknejok.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3iactcqlz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3scddrjjm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xvzanzhl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3kqjdlerd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3mnycyuis.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yyjbuzfr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3jhvkvqrz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3doqffrbq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3rrttbhbw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nkeyzxxb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gafassca.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gudipuhl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3shqehake.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kebseyqd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ditwwjke.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eengfyin.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3iatspauk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tgtedpti.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3uqhawshv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3uprtawem.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vkioviuv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3cxjrxkpl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pkneqdfu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qloeabbg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bvevjzws.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jfgqkryq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3euybsdpb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xlxlrzis.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mvcwnrwj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjgkymkl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zneubuhp.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwwoivkk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3andodaug.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3nrhdtjhw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3mfabhevu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ikxsrile.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3uffvuodn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sffcbjbw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3orehovvt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgjyqizl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vhfhmcem.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3ldbyiqcf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vuyrrkyc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3zuphxjcg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3wpswqdlg.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hkokhvkj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ycqpwzqg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwminxk.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3sdowwtgm.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3jmvkilgr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3nfuznbpi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3aybxbqwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsqmgqww.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ksqyanpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxevylww.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3etbbqgan.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3aezlvmur.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zhnwgduc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xhmzjyvd.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3qfjnefvw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3xrqdwrlv.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3oxftqhhx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3gorzwrnq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bjuliqoi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xjilypyk.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ovbayabc.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3lxlamfbx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3aynfzvht.html

);
来源：http://www.52xcode.cn/Article/details/gt3wlwwgfdx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ysjkpvbe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vnmaqxzm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ytilhebi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3eqiwimnu.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3tkviimsl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ipqggmes.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mqorloay.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jqtlvqsz.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3tvhrxkfw.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3refitsbj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3uujrzfaw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wbkuspuh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ibcvvqbi.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gditjnrk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3pkxqkixt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bnfxjjnl.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3hqsjhoxs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hlfobvxb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3dxolrwal.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3tildjkgv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vstohcez.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tzuptuxm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oighyddz.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3fqwumuoh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3eialapbo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3arjumadh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ajslktba.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xqssntca.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3jpquubte.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xjgpowkp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3iojztkai.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mttwrwxm.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ijebckjf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3heolctlm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3vhivnwth.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3cvjjdzbl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jxarisqz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3cmqwwkej.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3tbtbdnnr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3cftkrxkl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ftliocjb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yxhrzljs.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3nzisvrwr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3iuwxmjpn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uqrvopbp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhmbqrvk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3baqkppiw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3tsomletm.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3sqjvymgl.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3etvaxujo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dcmfdmfy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pbapuhho.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3dupoxgwg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zlnzsibc.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zoacfwze.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wdlwtqbs.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3gqjzauej.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fxedzrrs.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3nbjkcjbv.html


<!-- 参考信息 -->