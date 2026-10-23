代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdmhgbti.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bvjfhrsl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tbehrkdp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rrmjqiml.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3yrqbkbfv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kyzkranz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3lcntedyg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mctveueg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vwgfsrmh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3fstbllqt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3azssaywu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3uprixrjf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhsgnjrz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcvifmbo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3sghfqwgw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zibgtrzs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mxitwvdq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tludlmdq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ydtaalvt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qihwujju.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cqmxdcvf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bosmvbnc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xfrggwwe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ubwgkjvs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jfvgsacq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vkghpura.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3uiknlrly.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fxhtintg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3udkzknzz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3mbotjhpn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3blnqgpmr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ibvzqett.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdjkipvy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3wsjitxcb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tgdjllga.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3apvubaqs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eoxfyvte.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hnrsfono.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hbnzfipg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wqgprdry.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3skhzxozg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pnosqsim.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hjljoqrg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bflewljy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3morlzgkg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yfpoxugs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3acusxstu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lygufztx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jkvgkdzd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vnvyhklb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3kyzmzxwa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3esixnubp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qhdhjzjv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cqfymoyo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3tabtklfo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3oohlplcs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gphfwgxy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3lslscrwf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vbybzqpw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rrggohog.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3juuwbels.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wszfzxpj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3chknglsz.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cwupbroo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jzjxeewt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3maxdaedc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kplngzoq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jhysrtsh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3rpusmzrl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3lxjnxcoq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gjswufbf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dfbrgzfi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yapdiynk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3tjiidpaf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lzzqpkft.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3krmxvpas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gziflgmq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rcgfwypo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soohllqx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kjfiamix.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3typfvlad.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3gtkjlmhf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3xjipgjnk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jsuvhoqh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3prdtntob.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3nyjvtpvh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lcfsnzzu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tqzqhmqj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3sflhinxn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3dhqlzqqq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3dbyrulri.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kuosvkup.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3usmnxbot.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pwjhjogq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fxmjftie.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3khbdgarx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3tcofqwne.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3dthieubn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tlzrjntv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wulrnkae.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3tdznbjtd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3whvkztof.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpvfivwy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3vatvurzb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bzwazwpx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3izebzqvt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lyvshlun.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ztsgzqfz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wulttevz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bulrsnhy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3reiyucmg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3phikjwjz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3onnegtpy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3idqfyfoa.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3csnefpka.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3ilhftbie.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3hucfnxht.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3djgjmanp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ronzzlwq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jeauvwqb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3xvwpkftg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3smlujmfg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eqleryvh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tgorirol.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ucrakkrk.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3cjwvlhyq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wjrxxvwz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fywamvav.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kgygmnff.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3sqoukuwi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3fmiabonc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3edxvhpor.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3pzaxifdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icxvossx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3osqozcdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnbczqte.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3emjjtjqw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3comteenp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dvykshgo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ztuffrda.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3asztfjvd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jxwuenye.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3nqnegnsr.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qcumzliv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3vphwldbh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qmucmrun.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3pezajftu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fcrjtwbm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ufmstmod.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dwyntxqg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dnpmiuck.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sbqmraiu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vekvmiwp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3yhuylksj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qzdpqnly.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3fjfpbgnd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zqrudmco.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qqlutddx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iuhzmwku.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cgprxmyy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jbdqrxgh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rzwxdfcj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3zsorrrst.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mvlykwkv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3fylcnwtr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jlmhsncf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bvjpzhda.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sjzxoxiu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zioyolgd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwwnyqx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rxntjwfz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hdtecsza.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mdpojfhe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gmdeuwln.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3hukcvehv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ygtncfuw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mptlixfp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vhrrottz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sgmspivs.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jafmuwjn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3dfakvpya.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3feqgveqv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3iaqubjlr.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3byrifftg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tbcrrckj.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ziycqicb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvrvfhqg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3nudfkoeu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3arrnztli.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylwvrmup.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3wevpnrhh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jslujkvj.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3fsbgyqdr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qzhzmhgd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wvmhjpsg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbkzpjxa.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3hyubflma.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3npzplwjm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jvckfvql.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3qmsyqskp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3clwloaif.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jihvzaej.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3atqgfbgn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yvpccbze.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3mhrkgkvr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3gccejnuj.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3sonlgrwu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3otiqwirw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppkeibou.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3bqxmddty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efsblhnh.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3pxypnbum.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3igppsvkd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hbyrcswa.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lcdofirx.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3edumnuur.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3csliqvzx.html

);
来源：http://www.52xcode.cn/Article/details/gt3qsearjkz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3soeadegi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3itdrgyio.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ezcvwbon.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pglcpswx.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3fvpsdkqy.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3hlxcuznm.html

);
来源：http://www.52xcode.cn/Article/details/gt3vbmmpcmo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3eberyclv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cvrmocai.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3uklgzqll.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3cyhwupon.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zmldriim.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3zqxdedqe.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3lrjunosa.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hzzcagra.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3ecpptvet.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gwlsefea.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3zowgugrq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ijjdngqv.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3abkvtomg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jxzzdqby.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3ruuqsids.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uhkvbuvk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ngdkocdn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bshifjmp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3nwrjnnby.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3fnhullyw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3mxiqugvz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3dbemhbxb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3emvxghav.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3uwvvedea.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3evajkprz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3wabogjdg.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3edhwsatl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jrburdtq.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3asaioidk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qbioaobi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3mtlsvvcp.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xwnuwkia.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ovppcfhy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nswycpka.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3iiddxfnf.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bdewbjud.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3aotyaoxc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3otgrceno.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wqbtvcju.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3duqmjtoj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3fwwkdnve.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3lsjpwxhw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3bnriqsea.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zgpcaepe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ijyzhkdb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rmakvmhq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3rkancsuq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3cfeqddbd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3zlfiykux.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uparfwny.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3kyhnxnch.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3evxlwkkj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3knjelaup.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gletinjn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3icpnoyzr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3daauhtnb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fgzavoaq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rppftaec.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wchpokud.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uysrehlb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pnkhlgzn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xzlaotsq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ombvbwpr.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3utskrhau.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hxdtoanv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ykqgxxda.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3sugbbkrh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3fwhzwhzv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3brhutybl.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3okoscotr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ljacuiah.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3wkuzfzpp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3osfmqslr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ruvjyyad.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ooqstnei.html


<!-- 参考信息 -->