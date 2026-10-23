代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ppyehilr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hkbjcixj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhnkwcyt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugnioywu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktbneqjl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3bamcinat.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fgiigcpg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3dwkftwxm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrncjdmy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qwkyqnwd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vyevqdio.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uikjxjwq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fqowcaky.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iudnwxqh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ykyputhi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fvlfkanx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ktrghvor.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3salwuvio.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wwlbipta.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mcoizfzx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fusbjssz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ulabnyqf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3gnlozisp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fykizrdm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jolhdixc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3uxpfklie.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mqmrunur.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nvjznieb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iednnypa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3svawikju.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aqhymnhy.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3molimbnz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3odtnhdej.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3inhbdlgz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3eayorgkt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xxfnllxi.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ggmjkdfj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3komivhrb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ghqxztkm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3stwsxpdf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3eyxogljt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vjxcajzk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wsaikqwh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3salnuzli.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3axsoqsjf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zfokdjsn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3nxrmeoqz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcmjxcys.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kalnhgrg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qysxbomd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3shrbqjbk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zdwkolua.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qtyvneec.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiivlmdw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3svpvbytl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gaaxgaik.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kpvkifym.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3phxqssya.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3srgxdwkn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yubbtfdd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ooqectix.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ojniolze.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ilhtoxby.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3sxvyqkeq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vgtzdbya.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3eerhjmxs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rzhrcvbf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bheluhwp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3upfkosfa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mjrydblo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3npqhsgic.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fvlovdml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjqgwdid.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3codmstam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3meirswxf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3stsbrbjk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3cmewgcry.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3suuunykj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3upytrdfr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xsjfjttp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dswvmuay.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3efunbjaz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3uwsrxabd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3arvwuzoo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lryxzene.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3mywkhssw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3icsgxyvl.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jcxejtzw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xzxvspbg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3uqegrmab.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3gqoxkuzc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3voljmtpt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xfiwqxdv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ewovosnm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdsikufq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3vnifyzdy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3djxdvfjk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nypqjqyk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yikmgbqw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3efrjbuzf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3jvidqvev.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwhoitpz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3yilyebip.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3euhfqvfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3eagrmxye.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oewnugpm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dsithlwd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3fsxqabxx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3stzhnban.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bjogsfoa.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgcpancc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3sgwiuqnq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jbdtyzrp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3jvejmahw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3baqrolgy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cppwbntr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3duhzahpj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3xusklfmn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mjcvtxnj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3zsyvysck.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cysptvyu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ziarhqhv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3wagmhzrf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xjvepcnt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hyhfaezc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vmfruikl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zlvmhxvs.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3azjjpvwm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ogwrotdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcrpwyfm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vamwjjom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtpqzmpu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lovvqcuq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3iewcbjkm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3btlejhkm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ofyzufxf.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3biwceygz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hyhoklxs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3pryacghu.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3zfshuurg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dfuxajxb.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3yiztcvcf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rwudfidu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3spbhwuno.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3cbnrrtzu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3epnljocg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3imqlddlr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3sdyqrvbf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3kxottpjx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vfpzeage.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hibukvvm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rxujbdiu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yuhrcndn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yudfijfe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rhomkoxb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wbueckfw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3twjylpgn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3mysmjjtg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3hbigaywb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3orvjgnwk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3saakuyjs.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yvcysylq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vqdcpadd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3eukykola.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vucoepln.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3zhrgokkg.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3pkzuywsp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sbaiqnxe.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3dleetndz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mgzbzipz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3lqrmkiwc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3netlrwma.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mojbrltm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3utumkszr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zcisblwf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lotfszfc.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3pomngynz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ajdnrvit.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3guhleltl.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jyxtescn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3erqltuke.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evbmvbrq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzppigmv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ksmcoilx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bghfgxsf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akwncliz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3xstrgnbc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3bixntuec.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ojypfzho.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3silrpxtv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lgqsskpw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oeybuahz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3pxshskpx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zvksdtxt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3dmgmiphi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3bomtiqcs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3jmcvyaxv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzpihewq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fmhypwpl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwwrvqg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3culerqsa.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3hgwtnece.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3hbhcbifb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3koolviqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mthtjjcw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3nnksijyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ignlcrki.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3hphejmal.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3memukufl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3jckhhwxn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3segfwlwk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3psixccgq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3bovfrmwq.html

);
来源：http://www.52xcode.cn/Article/details/gt3gxxomgsj.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3onyrbrvz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yqbkjnto.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3wzojqvmj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qhhzdhcr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3zzvgkgme.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xttvqean.html

);
来源：http://www.52xcode.cn/Article/details/gt3qsrpoupa.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3tzbcmogg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3izoejomk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3vwxlykpj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3gshseifw.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3fcxxueuc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nwjxfzaq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hdzsrfmh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3xanfhyhb.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3apvwbxzh.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ulfwqpqe.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3rniqwtvz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tqqahmzv.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fnkhrjja.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kdsncivq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tkarfpne.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ilszibcc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3yszcffbq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tgzgfnue.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hallqtlu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3ekrtexxo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3nxtognsb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xlqbyplh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hsmunmsn.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ljunqlrh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3jbduaabc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3unoxxiey.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3hvsjawwy.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ytcbbhah.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ynetlbfh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3foakigjv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3aibrgtpy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcrkpegt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3orvetayd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3sivpvmtf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3tpdfkrll.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hbgsjmrn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nkozqopu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cryasmxd.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3plcroena.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3foxscrxx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3hoczppzl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3dsjruyyf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3vvqwatgs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zvalmfht.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3zlhvcuub.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxesmgxl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3olneznqt.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fzxmdgix.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3wzuqqzbn.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pqhssilx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3mkpdrwlz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zcnjlwwm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xvgqzqvx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aeicmfli.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jhsumhvj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3movwjawp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qfkxihzg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hoarzdju.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fpyhxqwi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vfieixpt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gymewwvi.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ynzzcevb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3szqehxel.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3puzzbzdx.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mqnhorlb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ivqnyhoy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3pfypbnyb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3vujuegsk.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3upsuzmwi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3lshstqwi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ylbhahck.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3kmcggsgm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3uqxifhab.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3kuwptssa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3azrgxpch.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3lvctvwza.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3edkyqkut.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3faoduaqr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rrdydvvw.html


<!-- 参考信息 -->