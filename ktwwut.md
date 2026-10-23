代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lymifivz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3njidptbp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ofwecjuh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vhkrqznc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3uzcivuik.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcpsfuz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rxxwpitq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pghtvxgd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbmvopij.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mdqfqlsn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zihfcaho.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bnazghrs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3euamjwky.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mdtjkyil.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3aibrgjyh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ceoyxewu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cmkwjjos.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lcwydwch.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3duidvwrs.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3czloidgp.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3khnkfyxl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yhizzkzn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rezguvyv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3klreeahm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ybayuhwe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmvzhrf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ubpjzdjy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3wbnmpjfh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dqowklza.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kjubfomx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3emgegrwl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3yavpgclh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hlilewwu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lmeljbrv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xwcxbzfl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zymissky.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xazxhsum.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mtetuauw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nprufpvl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3erhuffyl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xdrdlzvk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wqcikroj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lfdmdllr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vrhxmhhe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3yrymbrpg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wewnhhjm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3spehppge.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uumvfnsb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bxpfaibz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3bndjfsyf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vivjvxfp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3muegwwdb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cukzmlwj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3elzoajge.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zdvyovqp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xcnkxrzo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3srmkymyd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3oaprfdqb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pnczniwn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3iyobajbb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3wlxblkox.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wcfjjaxr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lgorzlfg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vcbqdgdl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xjxsjjlw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3chknrhgj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3achhfsph.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3yhbhgmip.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lnehbvbn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dkrgxvxv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kwzlobcp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qkfyeqca.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3pcldoidn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3cciuejpo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3tlmrtvsk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ujzakqtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bquibzef.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3adugclmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axiyocgv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3rkeblslx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mbgrrxng.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rxtafmwc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3khbhgjbk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3saotqvsw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3sezrphrk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wmlpdjnq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3opdjqkkq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mfpmithp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qakqngnr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3bpzzqdjv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3kttlrgzk.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yllpndjd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ayfbfrkf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3cgeaaiqv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fukmfuwa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3pombgfik.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3rulhuamr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3lindrhah.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3schaducw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ungefsxx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3iuavyszr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aqxwpyct.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqfmvgyp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3osncptuv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hvsxedfn.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkgdkdnw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3sfuzgllx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3mzpthayo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3fjnpyrmg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3czgvxfgr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygbkqhbv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ylpbjlqi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3afrzgljq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3mkpwmzkv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3auysuwmh.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lovnsvhk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bypzdqxr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3fjzavril.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fsdggaqu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lnnofxns.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xxcihvhy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3rdlyjuhy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dsemekli.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tenvfpjq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ktkkutdh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3fcjsiebe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3cdbjuhfq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3auybsomm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kozgevhq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3uoexltun.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rfjfaznc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3uyqqkkzf.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3utwilvkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcoierql.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ittrrhnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbmchuka.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3npjoophh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dobqortp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bppnezff.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3qaaniuny.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pxdomjuv.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vuhhyedk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wrxvetyx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ctuljddj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3pleukajk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3bmggcesb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ercdhokm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sumcfqyt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ttmjwdmo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3thayaasp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3thwnhzkx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3rkugqexr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rrrjyqfb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lsojhxbd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ficvqtzk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3qsqkmaqt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ntevshvg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3udbddqcz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cdqhruqx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3waondtao.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3nvbseker.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ktnzbqvy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3bcgphuxg.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3skobjybw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cboklwky.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3guvclqjf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ojjjxmdn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3rpripdfb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pblpnnmi.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3boozsixr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zcsumxop.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lwkjwqlx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dhbdbvku.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tzibvlfx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mcfskqzj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3hghnfero.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yhcmvyng.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tvughqvo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ygsqrwbv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ndbbldva.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xvdzbjen.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wzixploh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lddxjulj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrhbtefd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3bkjrwwck.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqzusfkm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ciaruxnj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3aoczqxjo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3fhxjdagl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ugitdlcc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3egpwlfta.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3neaocnry.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ukpqlttp.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ydbywrqe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hntfpvuq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fffkpnsg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3hcrtjshn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3vqkmqden.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3uvsggegj.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3oddgmaef.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hiqrfkbt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jwnvoqkq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3seyxqvrb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hdvukreb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3oroxpzog.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3astieahg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mmvzrrlb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3osbyxbjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbosamuq.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3inilgweq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uphitcmc.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3evysvizr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3wffpvhbv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vdvsmjob.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pnznhkyk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zjlwkalk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tkxjxzrq.html

);
来源：http://www.52xcode.cn/Article/details/gt3oyfpjpmc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3koyqiekw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3eskhkyop.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3zdxvdlya.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3obdlmtwy.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ezwayvjd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3kgnmxuww.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wlboaabu.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vmnkvtea.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zeljqrwm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3egzddngu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3npcondub.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3mfufwlkq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3kundfsqt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3vwifemww.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3fjwuosbl.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3erbbbgwy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bslbtpdf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3tbkrtxbb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3yqryokdr.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3sccwidix.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3brdigwwl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3gqvzacwz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rmppqajt.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3uawmdrjn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lpivizqw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wdltyaak.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3xjdyefca.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3dvpjnbff.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3htdtnlpt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3eemtgvvp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wvtkvaax.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3tyldruwl.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3luqfqoaq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3uhzvboxw.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mbiohgou.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gxlqxpos.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kbcgdysb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3pdmrlbzm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hbbebcca.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3odeesnwl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3qazcswbh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3qcakabfj.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3aearbwzj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qbjabjpk.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3zzsoedgp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ucmmsleh.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3srfvuggx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ieqdtujn.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3alxuaoqj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ofbkdczw.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3haofbzob.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mzfypnev.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qqzobofk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3mnmpjnnr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3ghxithtu.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tdrmmszt.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwpsddou.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jitbdnzw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3efpcxjwp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3rburwweo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3whehkuzk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ceorqtcx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ykfwbkvf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3omzkhzlw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yxvpdjwm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3plyzqqxq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3tjurmowv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fasdrseg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kkdnodvh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3edroygks.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3udaoawsr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ibmqvhay.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3cjndyvnj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3sudfjqxf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3dvnqqbdr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3bqskgajz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3nhpmpcmz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vhmsbjid.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3bigzuqhh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3jloivfii.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3yxjhtnft.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bmntlmts.html


<!-- 参考信息 -->