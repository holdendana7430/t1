代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tygauaxj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2byfaqwhl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2giimjctg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lccdsccz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fahduyio.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pkhlkgns.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucxezxsh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2owdnmcym.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fepvxdyj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gontmpvv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2rsizqnje.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ocoiwklk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqybszks.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jarizkvk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qewgdvcc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uecvimby.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kzesmaib.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bmicvswf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yfzmbwkb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tuwzamzt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tuvmsvdz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zdsirvcp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wniomuza.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2iwdrhuxi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qgiyczuw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2osnzpvmx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2zfnzazaz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vkjtclwi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2owzjhbif.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hbumiktc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2eylnugrw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yzhiwfeb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wgaaoair.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2crvujysb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cwtndeum.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pcoyjuwz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2goanfzgo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwawmrqq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dvxavdng.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fyuksbhu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ichqfhph.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dejicwjy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xzuoxiss.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2locyealc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2jfpptbll.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jtyvtvid.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xownojdd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2guwuzfle.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2cvkxfkwp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2pyualdcj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2llbaokbh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zmjaqlue.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fimcqymb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2evewcfnw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2evkqvfhv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kmtnpcve.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zrkeczam.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2egnofjqv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iuqmuxok.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2apicytew.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jwbeesoq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2imfdqtzl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vgvsohqy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tyhheoaq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ahoqqrqf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xtedebky.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jcpkgnju.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cengeeqn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gfvsycdy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xxkuqtrp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2soidkhwp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zjochknj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cdakhuap.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2scfilgbi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qftkwdxa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wqealquo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acnocgpo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bxpmviux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdruhgcp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2krcvbubh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mhtgjkcu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2aascqftt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2dobqpzcn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ycwopglt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kfevilir.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2gfltqgnb.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2achhmmmf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2vqbrnuto.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xuaqfrjk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjjmbah.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2odoaicph.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ghhrngyw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2urkixuif.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qenloweu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2raamggjt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jovyhkav.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2npaszqhf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xicjqrxz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2onytvvin.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ctytobwu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2cnzoigmv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vemvdvdk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pacngfvg.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tfwhyfsd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qlbyrsnj.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgtfsaoo.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qrlqienw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ksoqahcn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ajybizfc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhsvcxr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmrjgabl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2oeymaxnh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2oaqgnnxq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2aayooayp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2veyblnwo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vopmvxdl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mcevrzcv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2crdvwyxd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2julwdbpm.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2triqznuk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2grpaclky.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vnvkqctc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2djdcfcwl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2aiwbjvnq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2sjrysxix.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2dnobcpnu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2deicckqp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2asjibecy.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2thoibqjv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2btkuwmxr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ggaldnca.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xntbkfhg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2itadqjac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duekexhf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qrjgjajj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jensblbj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vioroxmq.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2plnidspi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2lywlwvye.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2joxpdrwy.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cifsfais.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lcclakfk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2gokfhmim.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2fehzvifg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tzlvwrzg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kqovdwoc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2pxxjqbfb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vpvaohxo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wnmezdiw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mqmumaid.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jdcqbfdm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2iunyfgyx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2tbfbsmkl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dwnagvii.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ndkppfpr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ytllswne.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2msktbgir.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ulflvqst.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kkzqttlk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uktwtrat.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2caqjprff.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2syfyghkl.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2sksvvtth.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ouwflbqf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wodxgghn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jwrixjya.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mtbarosu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qilibkca.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wkgmidbd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2svsgoyff.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2weejwmnm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tegaygkw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2pbsjvnha.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2cdflmrvb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2umlqbysk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2kbqxuuex.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ybangyaa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gzusivpz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbrdmvit.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2mrolsnsy.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2slwbtsoe.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2slshypsp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2vgousnyk.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2agjiscmr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pxxqduaz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttdfcylr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fmrgncdx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2uocirhlw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2rgrfueeo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2libdbtra.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vonwkgrr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ozeredyg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ksguszoi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2smthcnmj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eapfytew.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2tnydxyan.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ekrwnphh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2odeqtouf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hwjcqmzm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2roxvtmtk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2mksbtvky.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2vjxhigrc.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2moykqquz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2waubtumu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2ggzjiutp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2jdpdahaw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2egxxiudg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2sshidlnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvyigihc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2xbgeempr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvbvivtd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2qejtljwo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2jblgumgp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2zbkbriao.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2dnmzuhwa.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2bdppskpg.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2mjxdsfni.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wfkhoxuu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2ndshwcxd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2adatrcvj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ahobuixe.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2iamcjbyt.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kcwwmzfz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2cegaixwa.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tkubdjgw.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2ivepwdzy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2lffgjnwe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2edlafqnu.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2kypaozvp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2nvgrrhoa.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2dofniwbd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ktmcpuzg.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2btiiedtm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2jtxvfznv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tqylgxqu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xysqqkjb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2kyvnnpjh.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2paflaqei.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xydfohib.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2prebqhxi.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lqarctqy.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ekuwlocm.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2bneclxjp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ryceesha.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lukemsso.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2cvnjiabq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2jesetdfc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2blxzcabg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2cpsdpufa.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2eafeaeac.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2gnzbgwaj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2epzswouv.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljunggzd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jjjgictx.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jnnnkewf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ovfvgrzj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2czigtuqr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qvurnvio.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2biylpphf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dasxxssh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ionddkoh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xenqbzhv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vxovsbyg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hzayidja.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ckkncupb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2qkurhvcf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dpgqxohb.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2uptkmchz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2chafuegn.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rygxizbl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wrxzewmw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2szngkbxc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jrbmeljb.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2kvkapckb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2psfachop.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2yrawvors.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gfjoxonn.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vxrxwzrj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2farvdeit.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ifbapisl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2boinzfjj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2iwsvmtfd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dbskfgxp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ulclnytz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ueiljktw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mpjzellw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2flzpwvxx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2mttfwvdb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2apluuijy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2irzaqcrq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ashprtoj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bpfnlsfz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fqbmnezm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hqkereca.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nizwsslj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tfogyzqi.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2huagiplh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ycsapzuk.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2sqrbyhkj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hhhvbroa.html


<!-- 参考信息 -->