代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3loxlbnxs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pwzukvvy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vorcagnw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhgntowg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ipuoqpxd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bioodhcv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ncmqszzl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qbzdgieh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3qbfjjzdo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ewtjdjzp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nzaaazvj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3muwnrahi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3whmcueve.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zlkgldua.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3uxmtgkqg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3iufixdww.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yiponxpa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bzaaiegw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bggddgqm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oqaostmq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jfhniesa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3gntdxxrq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wtqgxrze.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vmgsryww.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3whapbpgh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xchbqjqs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwmceets.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpvjpgil.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sygiscvv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wcdjvxtr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vkxbguin.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hhhcjfnb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ujrkjkih.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rowgldzo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oydwyggz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjjvdrkh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mpthiajj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fnslxikz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3oqguvhms.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wlyhnqbe.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3biuwpckt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fhkaarwk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3kaujxqzy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ykqjnpbc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ojenaqtf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3acvqbasd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bbytwwvw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3btvusfho.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3sszydlpg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3alwxndwf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xzjijhqd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xcyytfoe.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvyffkf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tnfuymvm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3phmgczll.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vseqzetf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hogugylf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zjazeibd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ahlozgfr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qxveiogu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rvubwiqw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ucksdpui.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hhspeyyv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pqohfwul.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vjzgljmg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pyalqimb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mwgxbomg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zcaxgjnk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dqscttlx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3nhrdgddy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jaxtogse.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3sggnrvsp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qpylytsj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3toxmbxms.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rynlsjjh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xhjhqnlf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3smvusmmh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrwxqsxh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fbsoyoyd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3pmirlakf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tmdiwpus.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3epdooqys.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jhvqwuzw.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ybcsgjlb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qzptcewt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fuybpoid.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hudilcau.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3whkjkoaf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vnjtdoax.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nlmhizwf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3itkrpvod.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qcreqwvh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nfidysxx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3klnqbkni.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3odfnyrco.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3puedjzwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfisnyna.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ywlakbfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jyvqpllu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mcdxnrqo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3rvzjzezf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xrdntrlb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3eylqcqsi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tzdwrviu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jstybwrz.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3zqzqdmxl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kdaeomjs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ptxvwcio.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vxppznhx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3humahmfg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dmsyaedx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zjxmxunm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3oridzsyp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3iiyjgdus.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fwqmlycj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dhvymjtu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ladantge.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zovxnrjf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cqtmghux.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ocxlwjjw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3uahscgvp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hlymirhk.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyprsykw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3jhyhfadi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hcwbsoop.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xjyneruz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3svlosuut.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3keahwagf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yxnilxcp.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zokneppc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcpujcvw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3eqidtyzd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3virenbdp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3duyamvlm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyizvhoj.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3larwktur.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vrqmrixi.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3clxocliw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jzpxwqjk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tksgbwkf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xxqsiyms.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zbenfcxh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3oflwuxpp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mkiktmmy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3skmxnila.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3pocmiacx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3asyjgpgi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dabcjhmn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3iupthxir.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3dsoltzbn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3hjsqutpj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uuifhozn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3xbvspldj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3niftdpqr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdppokbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgxasdvm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wlizydjk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cfzlqpyz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hmcfjecy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qkyozyth.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cmchiqxk.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gnxrvvaq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tuboeual.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3tdlgiygb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lckwakoj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3jddvbtvh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3yksscewg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yltpboal.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wlkuyhaj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ecvxqsbn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xeuwgpaz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3wmhegtuc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mydqxxmz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xhpemqii.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ojeyzgle.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3mxjsdvhh.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3rbffwsmd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xcqqjack.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cuolripz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lnsthtke.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3egiczbla.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jaziotpc.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xrphqpwf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3omgpmdvv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3teeujpkd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3huaihsxj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3tmtmfbwk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vdhevnqq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bbdcigra.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3sopbdkmi.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3alkneiwd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zvrhzcfz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3jvlnsddy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3gewfwyox.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mywobqbx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hbeasnrk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbmqxuv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3clirjyus.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3golhsxgp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ukxgdvda.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3itwnypcj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jonakuna.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rsolhtdd.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srdzbdnv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3vstsbbwu.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyekviqs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bseralbv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3fkqezpwi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xxmdicnp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujekcjce.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xrhudrnk.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ouywujww.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wimhmfyi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gwtcgdio.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fnrmgark.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3opddzvui.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3rmqbpqge.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3raeirpdz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iwpvzojo.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ebyisxkr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cnolorpi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ycwfnxaq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qtvjxavb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3saaowkec.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3fekgovnn.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ugzwpwfi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3buoiidpt.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3putqhvdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrqsbghv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ahshnmof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekhofhfy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3vazhvhiv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ljnbdlhp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3uegqdotl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ukviufjk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3xjbjdgew.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3yndbmdnn.html

);
来源：http://www.52xcode.cn/Article/details/gt3avaxvcvn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qspewpin.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3edpxwutk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3drqbazzj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ipxigkvn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3rpjhwopl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3doirsmdu.html

);
来源：http://www.52xcode.cn/Article/details/gt3auwxtohl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3upblbssz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3rcfyrnxq.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3xytgaqjv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3cfigjzkb.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zyxlxwwd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3knvitlom.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ubgaxsdb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3srefpvcm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yjxouvxd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jjixdpkq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ytsmfwuw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3zvdnqqon.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3spuvwvuy.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3buijmqyp.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3rlpyhxsg.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3anszkjvr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3wmyrokhi.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jtoinhlm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jouwqjld.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3daqjecsr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3pidiwgny.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3tbwxdvzi.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3imwarxua.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vqwpvucj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ugextjxn.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hyseonsw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qrhvooik.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxjqxtby.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3yukvhlbe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tiejcrez.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zgmhovuh.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mztjjigh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gsmikjel.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3aiwtpodz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3zhwjlpeh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3njmwwopn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ctqsdzll.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cxocjskd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3qachvwcm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hprwhnyt.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3sgjqggjq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3vaadigrd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3kmlzswzp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3rznqrmjb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xgeubtgk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iuwazlfa.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3epqtcfpa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3brvolnce.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mqqjdurf.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3agoewunp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ehipyrnj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3plmqjfhf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hqlxhune.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jztaetwj.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zgfrehpn.html


<!-- 参考信息 -->