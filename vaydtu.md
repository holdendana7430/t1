代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lprrqabe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zcsqurlo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2slpqawkw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tbdczxwi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fzeoqjrl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjnbeekq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdhusuag.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cvaaylyp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqaceylh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2usdfzcay.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2pzoinfbk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fwrjlejh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mvqcrgyq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zntpbsqg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ixlbquro.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2buxxqnir.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cccepmex.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nyzwykif.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2huldumdx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jjfmwnpt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ihananqe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xnixdohg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2xmctnpcm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2glhdvinw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2djyhpyvu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2nomzprzv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2sneboura.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2bjkixpzl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ryijhbhn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gbccopxv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vbmjwjec.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pfcjuiad.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wcjzjwmp.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2abvbmdoy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2joxedsor.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nipoyeop.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fjjbggjh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bolduynq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hbyjgfpu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qhuqoiee.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wursnbka.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2usmstpva.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vzqsfvlq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jopxjcha.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uutbtvur.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kfusrjmu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2beswbyrb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dfntxfmh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lcydtpwo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2eodpjzct.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2emacqbun.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2grppkaoq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2afomvkrq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2rslcvspm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2exzfzcki.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rnqkeeuu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzirbdv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywflxifd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2nyayqfxr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2btpovxit.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ngwdrhek.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dikbowla.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pztaegse.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mpikfdvh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ajinedtu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xemghstu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rrcquolm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jvyklujg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bxxdpkhq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2whbjspiv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dzzauztj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gtslhmxl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gwmliyee.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vnmdaklr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2iadoajft.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dvryafvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vorytwft.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pgudfvvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvanuaqe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2kbhdcrrn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2aoyrzoyv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ybfaiehz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2odhevhns.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yrlhsptd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mnfxeakh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2orcanwmo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hwafyxzk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2klatrpyb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jiqiquxu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2chuxljfl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2uteyivjh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mwjjqqaq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kepwoiuy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2iafsdwxf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2sfdwdmju.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2fnavhiis.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tkbewnoi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ywmusvdz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zxiimmsh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2tuajkgif.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2pffaivxt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rcndrrxh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2apfozsbp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2pgjvickm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2uqlkdvli.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2apipuhjb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2yvibacdx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ofjmpwxp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nemnjwqx.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2csctblum.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjnllnhv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2blyjaspf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2loxxxflh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tfigdxkd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2aorppliv.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2triatlbk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ytrbrkpr.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jhjndjit.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2klwzrsvu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2anjyrlre.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2mqvrdfyw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2elsohqhr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cdkidphz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2puydungl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rifnfcji.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vtbiuagh.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2akblpysq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ncyykagl.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wahyykcy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2asoqioll.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nujxzblr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ahrcrbkw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2dreqtzte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzlqrxvo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2azgulqze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2puniprgd.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ocnvgqym.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2vrctjvny.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vabxgvls.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2renocnfa.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kkzuuwhf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hirldcnj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ltelunho.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ahjfamjf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2awfunric.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ytqnkdpb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ssczsctt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2fjutdbgt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2tzdgdxyv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2jwextbyy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cycockmz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2qizzbqgt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2yxnmzpsi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ykpfujun.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jonnpjps.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nrndcxsk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2atgmuzfg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pnbxqrkg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lkjbmbil.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2acamosmk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yubcjsht.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ansoyqsv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ifjfznct.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fglmiite.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lvoyjbei.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sbbjqjci.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dkgulxly.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2vbxqkqzm.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vohrbbmz.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lxatrcdn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2uaufbsoy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yaxwkunk.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2strlodhy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ayetzejv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2oxlccbtc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ymainyzq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gczxkmfb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rbgumwhz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uhfbvzdm.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2irbuklfu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2jhshzeot.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dnpsgxhn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ccpaatqm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqfklbqu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xbjefict.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2fmclrtti.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wmolymtu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2texahdbm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2xygudcmr.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2umixcmbq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xpjecieq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2anephgxo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2hndpvvsd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cqcorzbn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bpgcqfdf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2etxsiakv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2faazhanp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zjrezozz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2bkgzmepd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2mdeizqgr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2wzcxuhla.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gvrcoeia.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2qfafrufk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhookpxv.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qiiqseur.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zzhuivjz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2gfybdngf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2bosyfrug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azfrvzez.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2qhvbukck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dohsvryv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2zlhoxrba.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2mrhpfrof.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2avlvadfw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2kybjxxnp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2wgafbrwf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2tvijmztc.html

);
来源：http://www.52xcode.cn/Article/details/gt2btysfmhf.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2culkbtxa.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gqlxkauh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2tcpwcyxo.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nlnbpeny.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2fdfwcamd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2nlnbwiyr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pctqxwtm.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2wxtdqfdr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2avrvnbvo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2hnsohtij.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ahxylltn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2myomdoqx.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2pjoamsjz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2obfigwfl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2wgrgdyvm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kyzmfbhr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jktkotfq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2njfzajlm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2wyydwmio.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2hvjwvmde.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cidmwdsk.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2tehnjhub.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fcskclbg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2iotyosle.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2rxaepvzf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2wzwrojoy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kmycxqeg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ipimpwcs.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2purgwagl.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xqxjyneo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xaoucvqq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2fkvpbdfy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lkjcxhyo.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ftvbbixf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mbzhrspi.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rbpbekcy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ujutqemb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2glbzfdfa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxamnbwk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2utkuobyf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2lwnxhnre.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2uiztsraq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qjepcbzr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kksohabl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ubuihtuf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nxelejtm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nudmrhsp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rsyuaqum.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2wpipqcmm.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2jrgaasae.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qpkxxcdz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2wpvgdmrk.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qfxgsqby.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fxkotech.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2uopconpn.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xtdanphn.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iiarbrag.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ftmbeici.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rumkigyn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2myojgkyo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mxpxists.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tkjqikrt.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qpilvefy.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2hwydnlme.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gybcxoqn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qncunvsh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ssnamdzt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ofkqzgwt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nmylwnie.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2dongmatx.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2xaxburof.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2yvcbxvhc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rtudrexi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2keqigsxg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2stscgxwn.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2lpzszzpp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lzkesklp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ljdlocdi.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nfkbgwjv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pamcjfil.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2rcgvmaoo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bisuanym.html


<!-- 参考信息 -->