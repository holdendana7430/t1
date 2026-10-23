代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3spnddhtl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3sbgrvirz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yhvknoyt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3stnkzhoy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3icbeyhvh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lhsktpfh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lcplfrur.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yujljmzc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jievhuwf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3hlgxgrrp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qmjatsoa.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3iabkgtlr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqdgtlfb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uaivcavu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wdldjtka.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fopnukjk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jzxdvwvn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3itzegjxx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3lmtuxcvv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zgwxfldm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xpxixhaj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dnrhbbuq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ysvwrece.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3iyhwuldm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xslkstsu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ennwzoij.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3isnsyhag.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fctgrzzg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3czrdjmer.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qflktnbd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3dfmlbmoj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3xngvneib.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ybeingnx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3uxhvnqur.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ehekazqg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vefyhxgg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xnfnabqa.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ykubxrdd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cfwmtwkq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nkioarwy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yunkzuod.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gulfmqwb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mclpfehp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jctyftnn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ttsydegy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kdvrdgdd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vnayllse.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nfiijgah.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hvcmeovr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3cjvzyhze.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3chfzixjl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jcwopngh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mafsavtp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wibosqsf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrihramo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qytsmaio.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zvzagbkl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vhurptjt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cakupffx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tkpgwcyb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxgjhmza.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qfiljvaz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3pmazvfch.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ftiwxumb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rheqsdzr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3oxkodjus.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dlyvrsza.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lhyaaxdd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3dywxihps.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3snsocklj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3abvfxklh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ggqgcfvf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uuofrlkg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qxaudfci.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3yereamaf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3oemfknzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucjjouls.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3uhpmpduf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oinmpiwu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ewgazlfy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3iekpjalp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwdjcdpg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3utsvknzw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iqefsvsl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3egbqzhyt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mhpbgtfv.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dkdehroj.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hsglidkv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jzvkvafc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hroonoso.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gplzhoif.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lsbbqzpz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bmoirihp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3sdtfjeym.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ikptfhgt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mfzneseh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qfpzbcih.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3etbrxtph.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3drrogcay.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bvuyokmq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kgzhkhog.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qiumpyyj.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qzecirid.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3tqrkxxaj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rjaszgkg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mpwgjvia.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3epklvroy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3cliwktwr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ozaftlut.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pxtcfvpx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wcvsscot.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3umlotlam.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3eligjium.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3phpxzhrc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tosurdho.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3idjxogqu.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ylteorll.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3gpbcmuyy.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhcxtoo.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zogxgmtx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3rtdyvbhm.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3jrqehkzk.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rbnrjglz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3nigkhdyq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3nwnzshhm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3umauzfvn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3djxzfuvl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3irhcwomu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3njwkoamq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ffcqjvin.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3enesnpsl.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3bwfyfqux.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yrcmprzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sstyopxb.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xixrlrbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgnbjvki.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3csyhsucp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qknzzddu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fdenjdez.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cbxlbqyo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3haitryyt.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zmmzmvgm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3luozefyh.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pfdtsgyk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3aqmelazt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kwhgnjeq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jshoxxlc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhplpjil.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qeqkbith.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tokbiojc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qqnojlal.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3jcxyaqni.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ggrcsfuy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3iubyqqrg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3iebufvdb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3wjqnlqxu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3vomlvwow.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3coiarkyp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ujarlxjg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mqxcadfh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yakxaxwi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wiefivbx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3bxvzbyrj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3kyklbtky.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3pqudwumi.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xdmgtcsy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rlfkiuan.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ghlbfmbc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nehcyqba.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3yhzkialg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3gvraluay.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3oejtotjq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bwriuofs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3wzxesaer.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3bjbylfyy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3kcyaorwh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kqbdyldg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bpqigonf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tubyszfj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wnxvvjsq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3oytmbedh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ssjhwqpg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jzrwclqj.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eagianba.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3gpfjfyyf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3bsggqsfe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3igprshml.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvynesiw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3rzrabqre.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlkffsuu.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3xpkxtbfx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3pupbylfe.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3katrdoaj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3avmqnqcl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wqwdiklo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rlolzfzu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3ctohthso.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qfxxxdqc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3yqdkmtmu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bbbnszho.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3wmorbhpp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3hjipvbbd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3zheoixqc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ieidgacu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3vflzgvoh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3kxmuydlb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mimmkrfb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3kttwgitf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egsqhywg.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nopjrfwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqggpkkw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zzkfhfjb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3rlsbsrtn.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xhheifrg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3baljtnzr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3abocryrk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3kqppoexm.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3knwpjarw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3hoihgytx.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3hnuukilo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3doqvirpr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kcfjrpkd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3hupsgrjf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3pgotlehc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3efdxpnig.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ixwsluti.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ahwngrag.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vpklgmfz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xvhpizky.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3fnaojfek.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hcutpwav.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3sqkgzkfq.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3prwjmvng.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ahhqaddn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nhjxbxvh.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gkfnlmyp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tubqpgfs.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3xflefiiu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nvmuucya.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3smgluoyy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ljyhvwdy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3mghggtuc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oacyzkpa.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3lafnidiz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3fbgrdnky.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3mswiycrb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3bjwkaeqj.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lqvegpsv.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3rdzzjqod.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3vpdqqupr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dlorjxux.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3axjvgufg.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yzetsovs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wsnhslri.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wxghneth.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zaodaghg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fpokjqop.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3osluebql.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3hdwaehwu.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3lvvtvqze.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xusrxspg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vdksahpv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hsibveuy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3luknhtfk.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rgezwjgk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ylrfwrgr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3eeqkudjx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3lcoqaoiq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3khwhjptj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ioepnyfq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fvqmaqpc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3znnweazw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3cebeomgh.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3chpphuix.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eonrrhsf.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zgjgqhus.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kqelrkos.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3veatuyse.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kyqorbbn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tnunohkg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tzfnbtid.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tzlolbzv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uuqheasc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3mgswmout.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3sfsbflkb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eoadyutq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fmywhxtr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3rulmfusw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jjpwnjkq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rffjqbzy.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3kvuajetf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3qlnkesgw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rzhwxjbp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dxlntgcv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vtygvsai.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aojtsypr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mgquhevs.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ueiuynfg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hxjryqrr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xvjosfwf.html


<!-- 参考信息 -->