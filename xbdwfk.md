代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlvzbdaz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbtqvftk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3stuokymc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lxxhwwor.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ctmfguau.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xlwpkzji.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwmuyfk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bsxruylh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wqaqpbed.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gprluajh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jhnpdxtd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bvabmlnb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kjspkxsx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xcjyafbu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dckibvfw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wrcyfndl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrdmqffh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3kgojsfvq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bcdzwlxg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mtxgluqv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xbgwsjgj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nminezya.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3biajsint.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xxznmnwt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3thcrhhmm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jlsztzhd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gukxdkpc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jebkhwac.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fpgcwufi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ajyvkecy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dpzadgco.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3iyarumbi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wsqcjxfv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kmlkscrt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ufjwenhr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zvhuayox.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mtvcmusf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3giglenvv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pzbhkwbe.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kobkjqiv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xiaapzzb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hsywutgp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wvzjxcht.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hvrjxvyy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rvdsdyfz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dfuimptv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lezkwskz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3doqphlhy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vzmbndkh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3spoxolwq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jhougqer.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kncfwnzv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ffusnybg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ksotpfxo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bjgtiobr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ngvmgvwp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xficzkcr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tbtyqjfz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdepcckj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3opkvtiyk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mqycysns.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3yhnnhntu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3omhqwvle.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3uoluddmz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ewcqkyqg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3nsnmdcrw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uswvfmcg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vtssvynz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ckmzrdyx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fbtqmzyx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3anazpnch.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3lgkloqia.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tgnvhvlh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3athaclqc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zpnbcjqu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3veoqazvo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wriotbdp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lefkqmbq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bzyzbmfx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zogldcnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldwylzhc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ftzmzjpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbcxsrus.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zzkrkpol.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uonzmkxv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3esqdwqpj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cilsgajo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uofzrywh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3zhoefhch.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ytlgdqmz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zruaflxy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fwfssdxa.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fectcxxi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vtsyfzrz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qqgeqarb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tuxhpaop.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tjjatugg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zikngyyd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ijiubnrc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ybviypfw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3omupebsf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3hqmrgopo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3esvpfizn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3rqlqpsla.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jrsrvetl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ggysbxjn.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3idptvygj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3mewyaiec.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xlnrrpsx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mexgztsg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fmsfdrop.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3ppwabsmv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3cfbbplna.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmkeifen.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cttqyllk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3gghorfct.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3efazaftu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tudtuqar.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhqoptgq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3pbhemkhk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dtijfamh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3aiikajpd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ezqlfyqw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jgwapdgs.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3czaceqxw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zsucjutc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ehuiloyo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3duprdcng.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jkmiwegy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3gdskpehj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ajhmalak.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wnrxyhwk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3krfqsiek.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3lpmnfpfy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3dnbecwpl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hkrfxhee.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3jirsmvgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aewoxgwr.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3stoaklcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcrotzwz.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wwpncibi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yivpqigj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3eygkbviq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xgjjjden.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mgcqykeg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3lvdijccx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3mqizhykl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3qwvyammt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pzdnvsqn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3fxahorqz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rnbcpvdc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3nyltlbdz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3biqwgsax.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3wywlcffx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vzchueur.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3oeqdvajo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3fotmutwx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3tvgtijcd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nzriowwl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rvyuihyj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gvlutajg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qwzkmyhp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wscddzbk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gylhxepg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ansaxrjh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3vcysulhf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3sdaycxmo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3lilqjmsl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3bksuktus.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xytlorij.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yknysecc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3enesnqfa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3etuonpbr.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3uqiqdsme.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ggnbizsk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3urybbbdo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ucvbuctc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3kgolylys.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3kjqbbtbe.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3sboxjrhz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jppeblrw.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tcmkgzwc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iadsynff.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3lfmkjwgf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3arnozvoj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ywkrenjb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vwdqpile.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lazjylqn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3sehwvsos.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ybhsgvtk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yobwpwxy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewijdddx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3yiinkbyr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbzjympr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3quvfncgt.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tbmghqkq.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3azlarpdg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jqutghqv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lsxpkdes.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lndccxez.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3tdidwefx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qreaedcp.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3prijrfgi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3frkyyqxa.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pjrcgdcb.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3dwmrvyge.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3prufmawi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tjovlzzz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3aqlngoiv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xqmdwryx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tgzuzzog.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3qnjxwqnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbrsoyzk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lwgbkdug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3temlupoe.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3gyislbze.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qnqedelp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jxlljrbh.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rhcxcshl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3nzmyqxah.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uablxegx.html

);
来源：http://www.52xcode.cn/Article/details/gt3qjusxcml.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xxhefhec.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3aodvurkx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3xalijaoo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xqispuwh.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3ruypttqd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3savzovys.html

);
来源：http://www.52xcode.cn/Article/details/gt3nqwtaugi.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ndhzqxyy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zzrwlgxh.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wuympnta.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yfepftgr.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3tcjsmicl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3xbdsskgb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3utuiioli.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mitdlfon.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3shiycizo.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ofsondmo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3nhngqinp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3musvuymp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3gimdoftq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3bfjzxfhk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3fztkjrhx.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ahbydvzf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qufaxdas.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tfwuzmpy.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3coovechp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3mgpyecip.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3eqkjhjbq.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3dvsaemlc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ibodoocc.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3hcwwiqcr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ylvqisbl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3fhpgdgpv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ecqrivpw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pdnqgnmd.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3yhualyel.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bayhvpib.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3mcnuijbb.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lwvzocky.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pawofyfa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3pjnqgbkz.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nsxwecdr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3oukheenl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jdponsyt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tgwjttzt.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3osfxvytk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3zfuhhjzm.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ttkqlvbe.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3mgvjzirw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3iiuamnbh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3ykhcywoe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ukxhsnit.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rusiepop.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3navikivl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yxqcdhjj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rtwvyalu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3alkzryrw.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3htmfqutp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3biapbptk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3qhcxeovv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kwvzpwtu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3arliztbx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uqwwxclu.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3bvezrnyj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3szutyitg.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kmwrfmey.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mrmviixm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lxvuvzuo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tfmoilld.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ajuoerqx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3qgiepmzw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ejdvrypp.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3lysdjgkw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nqraoyiz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bpwpgqky.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3fzvlhwad.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3pxxvtgpp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hhriribq.html


<!-- 参考信息 -->