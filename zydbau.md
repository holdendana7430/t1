代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lgliuayx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qvlfwsgz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tyasjdvb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vxjlvrqh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fljmbuvv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fmizoluu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2afeopdiy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2emvwqmec.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dowanrpi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zbglhkzk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zxkkhklu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2oryympec.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fwqnsaam.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ctpargey.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2nwfgtfro.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2vumtvncz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2huwxdfmk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2plnfbuwc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rteeafxh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2niordkxh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jrorlexb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vxdetmix.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfyrsid.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lktcnnnx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bsqpdkwy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lnfidmuy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mjekrvaj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tqbgagak.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ammyutlc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fqezvgon.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rsgnwawn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zcsasagf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jcedykle.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ysltcnpd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eworcqbk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wupiluvu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ackiynhs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2svbihlmj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2mfczbkpe.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2miszfoaw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yavlfrms.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qtmyyrtt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2opikpzvo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uanxcyeh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nxzliibk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hlmasmkr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lbptpnde.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2semqiwjs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nftomzkq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2svhqdbey.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2zmdfyclc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2eygvexyw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2urkxbrfc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qgdzojfv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2apbgztzu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hdliuwtt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bwfjsold.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nlepeips.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2gdsrxblb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zgfsnkkj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cdzwofxu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hpkfaimi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jjfivhyo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wmhzyjra.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gseuhsbq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qfuakzxb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2irkrrkox.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2addifafu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dbquioqw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ptwtrwet.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ppsgmglm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2yccajjkq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aazutbnt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xvfbwjrj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsyrntjf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2oldullva.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2csspcciq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfdjommh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zamyxwgm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xmlmtxra.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2whvwxesh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qledmjhc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qascnkna.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kfpsgkma.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lirwvgou.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kwnpurdd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ebjrougb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hjanxaak.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ceblyxhz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wajtzmai.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2splqflur.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bumdwiio.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2irxgltgz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2lxlaugsf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wumtgkue.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gsmkgcty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvppzrqo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2xjrwtvvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avstgvcc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2idhslpjo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lakhkllm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2okseiuhx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xekcebug.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rlccvdzy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2skqftogj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cxywphye.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2scufrdfa.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2eakqjvrd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fktxnktw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cbsfcvqd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2mnpjddyj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ipmsnuiw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ebbjpfpe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2urmhvcdo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2umdfazrn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pdzqdtzk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fahvlwrk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yfapjvve.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ywsvkgul.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2escfktgt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2lcdpcsua.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vkuqgcso.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2apkilwva.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kgnmkhpu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fiawuhws.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2evdugxny.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ploggkmx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fedpdcsb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2xamkeqqq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qhjenqcr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzjmuilf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2tcynhdfe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nlvgedvw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2enslbsor.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qmjkmrou.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ribcunde.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2zzgtlpew.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qeihfxqa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bbnvmoab.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ekzrrqqy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nbhilwbv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wpihvzau.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ofqgpyzn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fagymjaq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2oyiyuepj.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ttmzwnli.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rezlqnzi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2chxmbwme.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nfzklytz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zvbhqkhn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2huucpbqd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2bpssshck.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2pyrrzevq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omkeedbq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qaejicxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovjtfxtn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ottmziqb.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2rwugytoo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pzuvfpho.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sucxotyu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iipkynxf.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2paqpqece.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2rekvhowm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ydyxkghh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gkvrbiar.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2xvomrepz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ytwehpge.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2hnwmreiq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2expktqcu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mpwtvrdh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mlfikian.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2labfihkk.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bjdtbxip.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2zrervhpv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2myiglmdd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2kjdrfrwn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fscyaupc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yccnsrsh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nhbyqqeb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vwzwopcs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lwnmhulr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fsqombrw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2fcvdiibm.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2aliehpxa.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2asxjauau.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pnrusifu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uhkqmaui.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ddxtqhor.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mvonqfvg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2tbtvvxoa.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2fxwfvxso.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vinkkfpd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2taguicyy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ftxoxzaj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2fffjyfel.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2tnnzanrc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vdzhemga.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2rassuyhj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ftlynrnd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2qdsbxnkd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2urfooxda.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2fohicxzb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pinvpgra.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2euafippc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dqhqebjm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgbbwwqn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kehwpwcz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zpbiwpgq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2nrrsktrk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2nekwkvip.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2yfbeutfo.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2jbjetztr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2ltyewtgs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ydsdaigo.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dpfpxwxy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dnpilpfo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2snjdcrgx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lltqqbeo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2shoryeeq.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2aenteiju.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2droarbzk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ygzpddbl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2rzzhrhwz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcfviuyi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2zgobqdmc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2dsrscuvm.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bcbabcfz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2opcjcleu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ishdoyno.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2uvzclckq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkexothx.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zmhplkhs.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ewsqhhzt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mgyropra.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wtqavlkk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2psizmrmj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2fnmszbjr.html

);
来源：http://www.52xcode.cn/Article/details/gt2zphvlkog.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hcucktrr.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2logafudl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2xkoeplfx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2tqqtuvle.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2igpfqgxa.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2vawtdnwh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pnqyxnrr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ynlbzcpc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qsokoirr.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2uaipgrmt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ygrtdvwd.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2tegsguml.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vwuhwwye.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pghpgmiu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2oxkgjmhg.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nxfbvqvh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2czaiojei.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ittrssmq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2czzgjiwo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rwlfbqbr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gyyrsgzr.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2emwrvjje.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bcmjptqz.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2nhetsjbc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wvhzxlns.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2rebmylxn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2nqptgivu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2bztbeckx.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2eixdfnkg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2omzqdopz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2kkrljlde.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2zrxvhgqo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2obknaksz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wvfhbgan.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xxweargk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2cczwjyof.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ymkngqcv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qzadcwvr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxwfjcox.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2tiejnxdw.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xyyghlem.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2khsiyuwq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pzzelwvy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2xjtsoyug.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2efdnoops.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2nofrmkxi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hgahheqm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2cjrfvwth.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2iqrsljwd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2yiwcljlu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2veffmfcr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hzocazpm.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zxoakgfm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2uzbpcwbj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zrzfwlnz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kukrreyt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dbrelcdi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ofmkohyi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fliwynzb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rcjvnoev.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ucmdtnar.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mfmwenps.html


<!-- 参考信息 -->