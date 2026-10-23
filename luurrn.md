代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hvnorkhw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mlpzvdtl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3avheifti.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xxohiboo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ixxgrhhf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rsynyqog.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3eedpykfy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bvfeedbs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aythgjyl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctjligzj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jiymeymp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dghonxyc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnngbhs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ypkgejac.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxrnwnb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dhdhdgay.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3achyfjqd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uruglknd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3whtxpdej.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wiglvwna.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhnolfap.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3bicishyc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3lwmjchur.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ejhiolap.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnxnoqri.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qdqraror.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hxreqeft.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3avhyzqtu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vazymiwq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uvfijjwi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rozozyzh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3iahgyohl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ihqsupqn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hlxzdgiw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3iixrqgln.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hztlvslm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qkceznam.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hsaizoyd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vubehogz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rwpzgxxw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zwyaziap.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ovmpuwts.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cikislms.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gzupmacd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwveigx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dwthxvsz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pekdmadx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ihipdpgv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vwsrjcmt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kytvhwzw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wwuvkoay.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fsooelhe.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ifwifgot.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3pyfwavap.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vywkpabo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bueutzmh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xkikvqbn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3imjilrzz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kuperzfa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hycthpek.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3lrmktpck.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dmxntawz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3meakvgpu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3upzuftys.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3howdtbao.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3uirkpgjg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zlmtbwnu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wqjrijvu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ygiibkxi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnuvvdwy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nariglza.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ldayoyjl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktwtevvf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ornqsqcw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kuxozprr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kerhfinu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wjaxnpjl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ogxxjvvl.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vsyddeqj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mncqlfql.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3fvdwsikr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zzizfqos.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ahkvzsnw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3iolkmekb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3luxudyey.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ezmcqdgr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3xhmcbujv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tiailmsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppccnyws.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3oevsgrrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkirywaf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3eqpntfwm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3aqjidsvy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3xlzrxeeh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nsabgtue.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tyjjcqtm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3whhkwdbv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ufcuvujf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3tzvlfjhi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3qzvkgchs.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vsgowika.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uixnsujj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3jvizsnji.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3trbmrkbt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3biesxayt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rxaoerbi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lrygtuir.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ibupmzzy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3bdxiwibo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3kacbnqpb.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tnrxikqb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3abnackco.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zdawuhmo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xuwkvtoh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3twdqtbwl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pfwhdtgw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdbwqjha.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3enuwwaoj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3owqbbjyz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3cvsnrolh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3tuedffkz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dubmuoro.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tibfjguv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xdjxydxo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3inftqrpm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3gayvviki.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzcumrcx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3qowvzucy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tdkvwqog.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3atzyblzy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ihxbqiik.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3apdbvhhx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ufrzrput.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3zstmfhbh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cxxibsid.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnkjdcvj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ckkusbzq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kkgqoszc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3txeuphzb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nhjraijh.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wqmxofdx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kzpvpfzw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ojsyqclt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3nhwfstcy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ymxvwnse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cbjzjcqz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3svnsprux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfrzlmqu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3tcxaewqj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3sfedtiwd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3njfptpfe.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3obqjdzwu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uumuomal.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3icxbxoin.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kqrmwaeo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ciajybli.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ussjjyxt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3drbwrvxc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3sukqxazg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rpyevprj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ojcfqdiw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qdqjwbrw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fccugwsr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3bqjeincj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfzzjbqq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rmxgypcn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kaeghhtq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zrfoubxs.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dettecaw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ssapauiq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iviihefu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zmroczbp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3iowqzikr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yhcytkha.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3wgwirndh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3gddqkgfz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3qugeugck.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uzbtbnbb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dacnwatr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3cbdnyqon.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dldstlij.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3ycnxoatb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3boqyefgh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vthfyzuq.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3tewjqpns.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3micekfxk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bnigootc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3avnbwhgq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zpyptjsu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3vdrgkmdu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghprbyty.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3qxoxcyqd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vypoqgvy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ivjqhqey.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cwcjkhyu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3bwihpxqp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3atffxzcw.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgplxuqk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dxqvcasa.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjdsyfkp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3iulbctuf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlixwmuc.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3zacsmmam.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3gfuemxdv.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ookbnysc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mabefvtv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rsiynhyx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcwcwmbr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dzgbmabi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3biiwwitj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3ddnvnmao.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ivsjicft.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hhylnbet.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eubvmtat.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3syarycgi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dsovhrfy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wpgmruix.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tozcnjxz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kjdarvgy.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3llxcmufa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwxubhwv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3flcbzmyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkstmigo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3qromjvhg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3oxqmwedt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zldodvpt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lxlsivdt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3gauvcxii.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3wgfrycsh.html

);
来源：http://www.52xcode.cn/Article/details/gt3uaaokfuc.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rbbttpgf.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3zrwoysjz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3tghtlbnp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jyiaknmt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3rhlaqtei.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3garucabw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3otpxpgii.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3cxkiiktb.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3lutnlvvy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cxfrpchj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3kyevpami.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3tofdwuwn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3pcwwatma.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tithophc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ggaztuoe.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bndyuacl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ysuzgliy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3pocamhlt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wsdvtcxz.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3nxrdvran.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3kifxfjez.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3lhuibfuy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ncjzifvn.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3cvvhpvow.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hzzymwim.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3jkmgehhd.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3qdhehzmm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3sgkfosiw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3opigfiwm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mggcdkgc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hpjffppd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yxpwsguc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3hytlgjmy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3epbrwldg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3flgbnbln.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3iwyabvce.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rjzlctdq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3pulzjohv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kmsrxcse.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3choktiqj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3jkdjvjuf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3vimnqknf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3vyethifj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3wicfxukm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3xncjklre.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3azzkjagk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3uojmntmh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3zvdzbwgk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3utxyxfwm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3djackwdc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ovhomrvp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3dnosrygg.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xaiskcmd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3aggjdivz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ydsuhraq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3kgfpjlmy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zmumonti.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ayiehwzw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtkqmdqy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ofhikhbe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jzxmuxrd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jwciyacd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bhxhblkd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ghyelbqr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cqkhixsy.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3igydgors.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ymohnzwo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qxnfqnog.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fehxotxv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jucttcqy.html


<!-- 参考信息 -->