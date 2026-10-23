代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjjsmspo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hjiwdvgf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3assnxuek.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eepiixlw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3akxrtbgu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gjtsewua.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vybvzgil.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xshqsjjm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvwdezyv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wfqzipzv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3spqwczgv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3btahmgoy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyspshlm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kkpypfsz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hzxcgmex.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ipsujycn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nuafiwvk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kwlqhjue.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3muixmvxx.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ykkndwpl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ieanqcug.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eonlfodf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ibrfqhqh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vwyudrnt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3diebkepf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bnbfeprb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zuqleure.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mmdetgts.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3axslutns.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3tqaawayj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ozictoae.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ckturvhd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3elhbyhds.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wvtjwxuj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fxyqrowu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gfhwedps.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kxdrpvuz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwedwgvp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ecukisju.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zpwiqtqd.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mtozwoyj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nhfpanrv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fmyuwudt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3plqrxbyq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vgawxcjf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kwjgjquh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3yrzuvfxy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qpyenoos.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zcrgijam.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3nbuyeryz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ilwrypdi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3yalcazww.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3juqumkaj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3nvknxxdv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmowlzl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3atibmmyw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hxguudvg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wetvwgiy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3awnlgeeb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3srhhbvqt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oeexaasi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qpistidm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3swdrszej.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dgzotdly.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tpsemujm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pyefkyut.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gwickokh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oqtzhrii.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3aqzajxmf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ocajeyuq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3toaovalb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3prndpnwv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rceorynb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3moprmxxe.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uvsoiqmz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3olfalufq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iohbddvb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3yjlifygs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdvahzad.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3aelrznse.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3iscznibb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ddtwjdis.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3mrfrfrpn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yhkjrnmt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qynohssx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ustfhpxm.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mpjkfixd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3klmmgfot.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yfdthvac.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kcupcpwd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vgjlfqyl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gpojezry.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3efsblsil.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wmyspgba.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3npbrsfyc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nlzekunm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gyzmzyjj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gilvkotg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3bubbjebh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ixvenbut.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3vlrstzcn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3pesoauic.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3dxbgquay.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3epjlybim.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ikeiwcet.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlbgmvrd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cerxhrxb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3lyzjimbc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3wtufycfj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3aleplgce.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3irabluhp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3abjfseuo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3iureozup.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ewzxbaod.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nukgfxfg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3znpvdmqg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ewugcbsd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3fsyboofp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cnlujosk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fmltolxm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pfssghxm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3laxbgaae.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dyioikbr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3qnffrkcw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3taiyetfu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wdarlrby.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3syhqfose.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ipthuspn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ahblnpbr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ocxkriai.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3fqdlvpuz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3mbcjaeqf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ujjrsymo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smrayzzi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnejuxsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fevjkxjv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3caxaczns.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3umccxvhq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3dlrbvjss.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3apycudbc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3svdewhbp.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mhkkzock.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3qjzkeeuw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zmijghxw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3smsgotwb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3cpzqpmmh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3kpvpgkze.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzuxkugs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3doxfsnux.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tczwwbtg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3grssyfnm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rhwuaypw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3whkwnzbj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3pzpgrtnv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aprhznvf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3sffmfbto.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ehtddknt.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3iwdfmzjq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tpceavop.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3byktvycy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3kajgistt.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ujkystgu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qluiepdd.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3oxnrxktj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3wbwtjdhs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wohtzhhc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dnvorszf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lublfgua.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yjrktizc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3fhsivhxr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kxiwaviq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lftwozmx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3apuypiqq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3kwzqxoaj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3fdyouuuf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3azmgizbd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zpntggdm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3wtqjhduc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3omvuzxib.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ucgzwfee.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3ckymeqfs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3hnvzgxpy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3xignzupu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yydngeix.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3umbrzuuk.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejlyqdii.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oovqzvdk.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3tcypztvj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xznecpqr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cktrwemi.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mxeironb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bfctymkw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3zkgbkxtv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dunvsgkf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bhwrmegj.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fdjtsjhu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3hmbzhmso.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qaxprlkl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3xfluenuu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nhntbnfx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3kvizmqhw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kiwqazjn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3hpumybcu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrhvaxlc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3uhueabcf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3alfqjwtx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3zdhsvvft.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3uwkdagft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zedbmbsv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ssfltcqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bifexugi.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3nkyrdzxw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xjrwxhci.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lfsqhemj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ekgewmsb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3izsgngle.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bxwsavdt.html

);
来源：http://www.52xcode.cn/Article/details/gt3idhtnpun.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3kwzzatdh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rwgbvfrp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rskypwqa.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fvptvith.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3pmpnqrcp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3rykomegq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3tkgacscc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3agbbbeqd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3levxxckt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ijmoxejq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3rshrecmy.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3vqifeldv.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qmbubbtr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3jrhfqdgq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3dxfjekts.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3lpcfzvqd.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vmczwzep.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zayphtln.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qanzrdzd.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3knzbrpaz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nocgwfhm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nfiacdgc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3mshrhfqy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3oeplezrg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ysjegimi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xdjuyluw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xrjesgoy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ssffwpne.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3onfyezug.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oprujfwy.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3vvgqvxtg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3zskxkbow.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3harqpjbh.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3ztvgmqoq.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zzhbxxtm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nektibok.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bqcwnnra.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zhabslpy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ivngqswl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3pykkbvxs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3fathvvej.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yeofrsor.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pgrattjn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3asrtuklw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wjgoohcq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ckmavdbt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3oydesxqb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3kjxoyvjo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zpgkzoaj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3llgjjmof.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3bctiayqb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3lttqdzwm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qsbloxbr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zivaguuy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3kbgstmzx.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3adsocofn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3beesfrrz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kjmcnofp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3feywxzpn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3dsclxobj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dyiccjnr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3twcfnhfo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3idxmalom.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pwdbekhi.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qzcfsxog.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rqoaqpfl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yviocvfg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dkazybdl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tuvrkvlc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3xkltdfdz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ufjefnmj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3nduocjrq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jxioqmyz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nnvvqkts.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3xxreugjr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gltotzfw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vaezgyxk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gohozphl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3ktihrsgn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3cqyaenfm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kyzxnazr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3mhvgjywj.html


<!-- 参考信息 -->