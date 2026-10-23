代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3troncefs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ilvzvnno.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ekoxjlds.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3bbuoitqk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3iaefdbse.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3struemcj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ciuokpcu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zjlrvmvn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvyuvlvq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pbzzwrxf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bnllzair.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3beuxhtbl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3dmtcrhmg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyoqbme.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vownhkcs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ojwbxjgk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsndilzy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rgfmlzdg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qwxynukm.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yonljhfq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouspytua.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mzaafayy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pdtjvinv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mnolyxmg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sgfcctus.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wruhhype.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3uafuruvp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3peuvbfvf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ggbuaudg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rvurcfyq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qfwkxknu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3iwyluwwp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yewbucga.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3odiyhuao.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tzxtsure.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3kujksmou.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vtjvkmie.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3pprqnjah.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3diobhjhd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pivvbgxl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzpyebwl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lwuecmrh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mjtwuebv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zmgkvyao.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3epjlytbf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ncvmcctv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3mdagfecz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mwshcjuz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gccepixq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qnesusma.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ktegwmpq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ujietric.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wpivmhsh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yxyblalq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3cnquezug.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jwtqcczd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3yjjynfgv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vwruhdja.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dcmaarpq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3uysobmdz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ihktphol.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eajhflxb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gykxcvpv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ezleelae.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hcqonsfj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kunnakjp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yaypvsyy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3iaqbbddg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3pkpoeqbm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3klhhbugc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rcdjhnsv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ungyzwbp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ysfdxroz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3whazuood.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dntutnvl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cjlzqude.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3knnsmffc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3qzdeazvd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3oyekjjli.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pzqbgfia.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tgkvbdgj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nkfdqmxe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kkkbksta.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jymnqycu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxuowrlo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ntngzclz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byyubknr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3frxbnavk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3oxfgboci.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ugfbgfxh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tqnyfsch.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3onrvdrru.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mgnuhjqc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3lnrdgpft.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fldbsnvg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3fcrymaav.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3uvipuspr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3pcwpaqkz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3hguimkpz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oljpngoy.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kjzroawc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bdjpqjfe.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3qcawjklw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hjtczxyu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3helplmfw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3bczacrjy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3vcqaskex.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3qakuphwz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3tszbgyly.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fqrfyszm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rtqbkdfs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zsqudxyi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3fwollhmh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3inbhencx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kafecfem.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hgeerzaj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3mflzurct.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqarqdpb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvwbjasr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hthrcpwt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wybrabtp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3nkpgafhh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvfeasib.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3nbdfwqtn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ldxxxlfa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fffshuef.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3pgwqqkkr.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ckeiveqp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3itvlqzwk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fiyuhahh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rslwwzfj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3ejdyqtcb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ieqszvko.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3xouarmzb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ddvdpkvp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ricdwrnr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3orjbcbxx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3uzkmlhdp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bdppsnej.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ufyzmena.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lzndnyry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxolkrin.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzwsgtmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjwhfyrg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uwewapes.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3zwhrnwuo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ckgmtman.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sjjzxemt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vazousxq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lgsjonoc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xahlcuwd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vvlpybur.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3iojtkixz.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3eaxlzzzn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ixhjquif.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3lwttzsqk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3tpceziuo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3abulpjli.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fobfycex.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3fuupwqju.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkfilaid.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3abattcmg.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwtaszjh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qwufjwbm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3vqhkkylv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rkafkjzx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hrabdhhr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3bwikedgd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3eobehpoy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3boulykny.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lliqwxxb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3idicmfns.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3oqgnedie.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3akmhfioi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sosmcefe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lgiriqzn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kdxydymo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3jpldmzub.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ebocamsb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kkggeeiq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xkkyiwse.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3huhqaloe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rtjtmsza.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3amdbfdkw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xrxwoevh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3trgxmlmo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ncywpfik.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ktszrwvm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3krnbbxjh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3yadqfulk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ugfrkhcz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfpiuamp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3ztigtnus.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmbscxrb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ubctojyj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3jpvsxuhb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3cfnozqkc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3witnakws.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3iddesojp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3hlidbkpg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3vndvhmuw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vpxyezlx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3degksqpb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcgvvdiv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3avcrjzpk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3qhfgdvnh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3yvrwepyo.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3bnyxzkvh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ydfjrdzn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sdakdoza.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3oossiqpi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpefqhv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3wskzrdkq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rxqcpcos.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ntaofqag.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3ytvlazvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kciaggjz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jzoznfjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztjqgxxq.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3lbfwlmwf.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3yzxasqki.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3cvicjgpe.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cdubhuwp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3gwvxmmym.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lkrxmrmf.html

);
来源：http://www.52xcode.cn/Article/details/gt3nucvmmbv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3kwogtbgv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3eobhulkd.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vsevpglx.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3gcqltruw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ihwejynm.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3lmieybhh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3prtdieff.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3bxqfyvgx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vsbjcatc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bflllytc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3errfytbv.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zwxakjvo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3mabfycuz.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3tyrxdbci.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ibbgbgko.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kdbshdla.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rkdsxqtl.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3pcleichw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3udmddcdh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3bxxviglv.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rwaiywil.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jbznfjaf.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bdtdshzu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3kmkzjbqr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vadfcssz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ojbamcpy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3segynrhj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3iuoztgzf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ajziynrr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tdbqmvsp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3otplauua.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3xcuwkfrv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dsxeeqiz.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rhqnhwgi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ybvbbxae.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yiuvaizp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3srgetkta.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3ignbzgaf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3oorgaxgb.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3rizcutvn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ypgogvsp.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3gkfgfvrq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3eceqxsmy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3usymdnzg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ksbmuuyf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3oenrnyzz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pfzfreel.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3aqdhnkqp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xuxcdakk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ijggxvwv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3jxsriyuh.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pzmkcvui.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjnuwgnr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3kywryrqk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3lzkabtnk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yctibcom.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hyypfwem.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3hbwkvmcw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hldkhwte.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hzwqyofc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qrhqpfnb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lrqijown.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3agvovalq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3ijvejmen.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xmpbugra.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iyrmuoqz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qgjsjptq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hvmyxnct.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xwbwqhhc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3etpdueva.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fesqwuia.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ffcwprta.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xpsdlofi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3kuvmvnak.html


<!-- 参考信息 -->