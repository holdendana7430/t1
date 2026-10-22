代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wzrazjjd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wqyjmrxa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gjlspvub.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jlziwqgt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rcdogjdt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2srmuibld.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yxutktbv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2znfudvds.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xtoimtlz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ajxdimjj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pmcseyxw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2vjmtvsvh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2zenuhonq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jmwjlldp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2gjfkeoxo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jhkgtpsx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwrilqgp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hsoiumet.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qtpjrref.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2limlvoos.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2meqvypxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ucdrvfvu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zzipvtni.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rqdjhsoo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lphzwzta.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oitwswlq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxgwlaql.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wctxcuid.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfvbtpfs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2nbxlhvsd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2glkrbbxd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jnxuhivw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rndjziaa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wrlkpuwj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xdezsaqu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfaipzne.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vzszqewz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xahcxavs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qjcdvfyn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lddkhpbd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2nzesfeme.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ltqmxfkx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ovrdzrno.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bgeotbze.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2guxozmmk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tjgtyajb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2lfnivcdw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fhflooxe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2oxeghabh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2xtdhhpim.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2msnmmpzs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2hrawoaau.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugimrziz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nhpvkewa.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lshkbdih.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kvjtzdgt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2anqnuzdm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hcwgidjb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2sujdkwxv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dorejayr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2keioocqp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ybwbptzh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ttfypdyi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cwwjweqm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ikizjtvd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qnzaazjw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2aufzbpnu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dmtiutal.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2tzofixjq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2plmudldu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zbrcsglq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkbtldwl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ddlvtyfc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qvniuaay.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xttaxddr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2lzxosdeb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2uqbftnmq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mpsqdnck.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bqzxgiek.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kjicdpdx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2qfpktzvf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kpbcyrgc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ubizyfzu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yhjovcxv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jyhdrzjx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fheidgrq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oumnhcih.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pksjkukx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2tlfphdyu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ojeupdai.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2svgwbfdp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2viozzofm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kzvovonp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jkevvdlh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2khobkcnz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2unlsrjvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmwbpgrf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2laryaxrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eizpfuqy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2gotkzogb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nvyezvmh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2msaulfsv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ekiupymj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vqxprfzq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yjzhkbeh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2vtzmdiim.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wcewbbus.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2caglofud.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xiyxnyrx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gbxttahx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2atpozndi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bwxqltim.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ubvlwssp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2demqrlsw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hrhsnsex.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rsgvjajb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hdfanljg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2vyuykjlg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjmmzceg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2mvdngrpo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2efkocwdt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2spmueqdv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cdjsmwbf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2iloixzjl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wgrelisc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rtgfniyr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2aflbzslf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ipvtjgge.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2bdqducul.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lypjkaqg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfsgqqbd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2szmdujnw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ldrhbubr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2evnrkxdk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmqpmkaz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2jskvgwoj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mifawswr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2amhrxtli.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xhprcqkm.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2levcpllb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rpxxhsap.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2nvcqbptb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bsjfnhya.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rtlgvegt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2qwupxqvi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2ntrnjrvr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2fpwovqwb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hxsecdsu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2umskzdje.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vsvyatsc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2zkvhecao.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2dmrohctf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hgviqsru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slvgoqvj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2czsbzlxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vostxnjw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2aavydkrd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gfogvpay.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2qctrietf.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ibupwtal.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lhmwcipw.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2citaslha.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lncirtjr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fxvclmkf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2boebixkq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2gplztxvl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2qqeukvqj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ckipskoc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2huhcloqo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2lclqfxmf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hpgmpubt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2fgydbnwo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2anpqkyjn.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2nflbzrob.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkuiltgn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2dewvkdnt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wylrxvds.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pxygeskd.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pdljxnla.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eudulnsf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2kyrvlddh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fetgorck.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2qldomrca.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bhajyzde.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2klwczeth.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rleavqzr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xwojston.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tsuddvaq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pgaaihhi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2afgbrtve.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hdqzhcqj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hhuyuysb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2gertbdwh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2fimdfnsh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2liixrppr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2gontbhpw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rarabnlo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rhmqzkft.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vhcvjniw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jbmiuwfq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2dszqdozz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2aairjjcq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2fonmfowv.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2byavvsyi.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2kkbaucnh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2kogskgdy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nfvgqcuw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvgbaddi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pqxiraxt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2yhrxvzds.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vxucjkgb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2karghfqh.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2osdchlfc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vzfhsvus.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vdtpmitk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2nyxrtmmo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2jjjwbdgl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ceftcwdn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cuizdyvd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2jsquwjun.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2schwirdt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nxpxohfe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2xhxarusg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mkqlltrd.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2didiccww.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wjqjayzo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2vwdmknkf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2lwgslqlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yikqhvtz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2pdnkdgdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdxuicmf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2wdavvkpr.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mmrypfbe.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ebucenku.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gctmhyji.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2dijaqiij.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2gnohjwwl.html

);
来源：http://www.52xcode.cn/Article/details/gt2fnoirexp.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2tsgrynaj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2dfvxwrse.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jkcmgcoa.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zaavyuza.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2eftpliws.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2edbrqjni.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ygypizun.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2dydlltee.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2ewcqprhq.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kwoiokvf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tkmnzhmm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ywccvltq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2lamagpsl.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2nzzcmxgw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qbnkacjm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2warfridu.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2urggujhv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2vmnoboro.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2tkdqhzcm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2bhknvnvc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gvebfxne.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2tvyesbwc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bzwrdzxt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vqhhfqab.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mrvtnjpg.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hnsgkkpe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fqtghzja.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2yuxyorix.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ammjgvwr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cpdjgncy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2vjqoxdrv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zqviovos.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2rljgeniy.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2srwjbint.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eryblbns.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2eoooshvs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wycmeisn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2etynjqfk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sjwlzkbp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2byyixsrk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2pgsecrzq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qvajjtbz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jmmenvjh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2woniptkw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vgepkccs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2swgvbisd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bdfnaztt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2oyfajytj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2yxipphty.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rpowbqpa.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2snqzijkb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zvfgyqqz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gvvhkwkg.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2drvfdkhw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2exxaqoph.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2rnnzwqms.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzjykrmd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2byulbrwi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yblwnjph.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wjsuiyyj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ukwyvtcl.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mipgrnho.html


<!-- 参考信息 -->