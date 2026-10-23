代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujjrcpfd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pjnckmma.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3shlreaep.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ynqdayoc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zopmwrhw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3okznmksv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mzxcklii.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohuyquzf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kugmjswc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3skpnqzle.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3vxxeregd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tjhfcyvw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ltyoaidm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vlvwzliq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qjpfmcjo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3twglxfkf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3objuuclf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rnxcpglr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3hbnwxgls.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3utkhgozj.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nddcsbgy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3damoqlzh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3objekcin.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3giipbuua.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jcckvrkw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lhofvrrj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3iiypoigg.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jpcjiqna.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vbbhqceq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3eupsuxyj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ofohaqth.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zegdraql.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tffwyesf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3qzohoagj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cppqsuid.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ndqqykvl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tzygwxnc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bezmeiia.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3tvsxgret.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rhciwgzy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ijxsstmg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bgxyiamx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tuglodsd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uwwebxus.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dnfaoejd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3occqxfxp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3pnwoyjde.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iuiiqksl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3afkfovep.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dnuvukbb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xgtqfvdl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfsdqjzx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wyacgdrv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3usoypqcr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hgypfpbh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3egjvgdmc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hbrkhynj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzeccanu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3znoelzka.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3lcmpcjxn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3neuencpt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3aikhywmj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vokcklwx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oozcjwnt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uqraffdh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ezabqfra.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rtqyfnzf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3exuyejjb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3viuuhcyy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3pmdkanmi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mwhcovmz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qulgfpul.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3whmfndhp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qflcgpcn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ywnaujky.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zhzqiiuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjovilcr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ydohwfgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwjskfte.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3pbyntotu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xdkymnen.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3axrwtsvv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3buktomwk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cbtctait.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bevwpzzl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3taowvjbe.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3uisyegnn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3lhyswtuk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hdqpwnff.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxfsejg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3cdwppwvz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3megidlfd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zaownxzf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3nhaqnvsm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3ssplpids.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cxbkdags.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3uhudjtxy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3sqstliyg.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nbzwiyxy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3pqaekglh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3pvuzcwxb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xvgwzfkf.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgdbqicb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ryhktgzv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ceyvicmg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktomkxrk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ogcpqjuq.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3uvnywhun.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3rfgpxdnn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnqmzcaq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3eqztqoon.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ihfhlihd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3oiuiizxw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3shwnboei.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3traapyhq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3awvklmoh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cuxfjxpj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ygtvqiuo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3foskdqjd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bppxqmdq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wjryvnpp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ielzrhtb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dyyedtvh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3euulqung.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3zgqxklts.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qywphxko.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hswfwdvm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3uujzpygk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qhphowfz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rwtqnbic.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yuoqsrrr.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3pbemseju.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ndwvlqpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uokoezbo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhdtzcal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blvxzbpe.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mnmbkdey.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3oyyzgkpx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3veftibju.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mbjcghmc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fpfjkiwn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3owfkjwtj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jssjtwsv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gkumuazd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vtxlvptv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nopcuvem.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3dzyylyye.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qbpxadhi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3bcvrixly.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3seuvsdma.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fqkzdovv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ugijbptc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3vofwodjz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zompakfr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3henqrmpt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3pxcpcovw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3lzltusdi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dawpuriq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yzssoruu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ihemxrdj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3bihvdbep.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3txvcdajp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3qubxlzvn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3cqbkjxuv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3cdeykhga.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cwnzwwhk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dzihzoxu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3kilfsfak.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kpliwzfn.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3yguhvfsc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3izfpgkyq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gszhlpry.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3pqxbuond.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3tusezpzi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mlkwlzbb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dglnejgs.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pywkfisi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mhwtettq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gfvmnfco.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3swnltfyl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3xarkhuwg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fwsipwpd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3swcbnirk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfbeursy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3wddajdwb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3cfupkfrw.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuumewvp.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3faaffpez.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gjrxcygn.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dkfrlgis.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3dcpzazeb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3fnrbibgo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kgslckux.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3huznfsfi.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nqkfyigg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3kirvzemh.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3kiyyousw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wjnopijm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3sfairyea.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jxgfnnih.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3tvepwrfk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3xdarjorm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ljczsdkb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjcwhji.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3diazlixt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3fsmqhcuy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3xakmyvbc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3gzomlwxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgfofvlz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3jrroovcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptesoccx.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vujdvhep.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xsbllfzq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tfbxvtmy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3iajncqot.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3lmqvicmv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3uxtegfdu.html

);
来源：http://www.52xcode.cn/Article/details/gt3pktadask.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3obnuikcn.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3pzrtjnlr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3eitqidsq.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mprubjte.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tvoxgmfe.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3hfypmthv.html

);
来源：http://www.52xcode.cn/Article/details/gt3byukrtfd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xtqizfpo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3sfcckrpp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3krivawfz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3udqlnjbv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3owfklzgx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3houwvxyd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3gxojnfir.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3somoclmm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vdbwlnzr.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eulrfamx.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3crfytipv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3owspzyki.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3haozhojs.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jsdpizza.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wadmvfoa.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3shqldrjp.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3trkbuvjl.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rdiofqlm.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3erkhoymp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3nfyvdsoj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3yxngeahw.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3lqfxtryy.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ftiwzgiw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3qwpqtagb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ayltirwh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3jzojpdbl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nzxsctqk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ofnxbvyq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hggqdxod.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tedzdhxm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3svfkozum.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xzvxgtqw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mdtonkju.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3czrjclbj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wyeynwnc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3kibzlgsr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tuyghuer.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gpmusovd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3abompyaz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3krezputu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3yucpquud.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3dzgvttet.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3axjzzrgc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3cbpffthu.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fikrcaqg.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dszvvtjt.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3ylnyqcuk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vdkpmbxf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3wvdqtdpk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bsbohrsq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zqanwdst.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbhtrqnl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mpkdxnco.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bxwkqtay.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fwwydvle.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qkmagdlh.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3yswyleyx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dgcptdke.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oepwaifu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3znqbggau.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mmpbamue.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fmjpuzvq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3baspfyke.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3nqawppie.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ovhriydb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pdavomoj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3dtskngck.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3netoghxz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bymfxnem.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ujiukgmf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rknaopxv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3znbzjguf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3appxjijb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rlvgwcbz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tundcnfk.html


<!-- 参考信息 -->