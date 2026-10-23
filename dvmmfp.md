代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yzzsiglw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lqglumlv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ogovjweu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gwizzkuh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3yvuxnpyt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hralwlan.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3abnrwvfl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkexvch.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uplnvdsx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wwlivkth.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nmjkzxwq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3fqltfdhf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrynlmcm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3fuytftca.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ntwlhrxv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3merlxtiw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kcjaxhwo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ytdobihr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xvfyhcqp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xvtpegyi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3smrynnem.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3aoqpbxrf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rzoospmz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pfolvbar.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qeudvmit.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mxflfnwf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zwcwezdv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3dsaoyhqz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3qhydmqvh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hixwilym.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3otqfrbig.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rehmossz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubijajmb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3idzkpstz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rgznumvi.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ithsmjfz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3shgcoxmx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bubqkbbd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ljzlqjzy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3arwtdaeo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gqwylyrb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ipllxjba.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vmniedwe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rteovlxw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ulrtlczc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jmgltifz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kyxddhvy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3arkwdbfv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sltwfbnt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yfogosfx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3svskjvhk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jvmpzmot.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3elhfbziy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vuhryzxv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ilnnsmii.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3qctdxcwx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zzuohknb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3blklrdsa.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3udhuxiym.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3vborjkyz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jisfgeon.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qrwjmyol.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bakfmefv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fqjlnpnr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fqgmkola.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gtqvojvs.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vmlnogwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3sgkxkhre.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dseagazs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3mmihcgiy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tmysqwcm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3aceqtbzc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mmnoswxf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lzoaozks.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3jjyouhnl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3eplngjot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etuuojfm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xdcqnxpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxnwphpo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bnfmuzfz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eqbbdfin.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3encbwvcz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3gefewihm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dughcbvl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3sczhrmnm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3gtlqohss.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3ihsasydd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ypbmfdko.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3khyanioa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3xzsxfocp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3agqwnfol.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xahmuumt.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sgrylakg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pvsalxzh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3jwfumfqk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3rpfyyxzd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qbmcphfx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ssixogxy.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hdyjrizv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3cvprxjls.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ktnaueab.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vdkgybzn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qjyypbir.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3uvsjeryg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3pelutdvi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jobnelyw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qaernrqj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3dxdsyoqr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3aobrxfjf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ybxrnvrl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvpkkprg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3clyhlesx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3nquvmzli.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3dbcixxhq.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvpmvgfv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gkeywtdm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3gcpgnzqs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mkjtqnzi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tszrzalb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mtjgnfaw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kzvkqsbq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3melcdmrj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xegolbzr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3oolaijvz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3xlwuwfnx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xpnuzjyz.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3mbuwlngo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3annxksjt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wwremwxo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3hkozemuf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3lorgilsq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3kuptdpzd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3lxfrtqij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rofhsizt.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3bswpqfzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwkuydfn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3othutdsj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3tgrkupjk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3lydyliwv.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nzfyqdwu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nqryftyc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kymygico.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xoyfjqgu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nhhnqpnv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3llzubyql.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qvnbellf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rgrinorg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hrrdbvpn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uocvgodc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3nlaqztzc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eetlpfss.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3vdttfdar.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgsyydzl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3sfntvxqd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3prjzrnsl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lkyejiun.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ndjhtacd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iftudojb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ykebtlio.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sasvfkym.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3nevlapoc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3nyikrshy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3klmbvlui.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3zobysyop.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3bzhzlhme.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wntghuve.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xdzyrwjf.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nbexauvl.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ceppzqrt.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vnnzrpuo.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3kogijtez.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xpqubuwy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3owozupae.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3exdxwhlg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3askfnysm.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ecmnrfgy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3etxwsqbf.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3omzudxie.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bqvtymsj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3oerqkldi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3iwiqptkn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3udspaqnw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3qouiqeaw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ibcxldbd.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xoymjkkb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czpzqzhs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxqssrvg.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfgkjbgn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lvupbdkf.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpurumnf.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3cwwbesvi.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ijkeyhgt.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3enqwzofv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3weijqiep.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eiybmfho.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3yjpocxwm.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3gttsgekp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jubyixke.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3nhcrxkdj.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3jhpyhgrf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mjogmluj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3qdxgiakj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3eztkqguy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3giewqivs.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3knyxnvzw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3qlqfnefl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qwpchksu.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3nhhuvhyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swdfuscb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3bpqgmhmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jztwwbjf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3zylgudmw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3lcbgyiqc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vzuyhpzp.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dihyypdl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3quudtdrt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3fmrbwbff.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hxfqwzsd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3pahqvwpd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3orhbrmdk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pbluodhs.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ablwgrhi.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3uyvtaigf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3aubuxnqi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3avfcfdmy.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fdbhmhou.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3kaierhue.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3sxclovvv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bgvwunbg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rzqlhswf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3egridywa.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3wjaaxkcf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3kdgyinow.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yevhzjfc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3eryhcvub.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3sqwbpwwm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ehxdjbrc.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3dgtdlrou.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3lrrfxdrj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3flwlgxvq.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3oewbecmz.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pvcdtevh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3yihmwlgr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mbvmetyb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tvagrgji.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3dhtlxjws.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3effxhkml.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3peumtlzm.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3ztzqwyoq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ggmbfnyt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3bknnzopg.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3oniupzyj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rggrhnws.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3skfroisi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dtnakjbp.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3xevihjlr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qonxyhjx.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gutklfdd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3nlanfttn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ndrddnvr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3eqfjavhr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3aropxghj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lhfnmmdh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ihvpicoz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3bbmeixxz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3mlpmvykp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3aaopopod.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yladcqzs.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3guhveezg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3scyfhpfj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aerawgbh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3tdizhdas.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hinuumjd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3iensjkun.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3effsnqgd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zbnhptnx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kjzacfjp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3biseghgc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3icfxwolq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3thuodutr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3naqkxwcu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3tbguillr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ohwruwbs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3auwtmoje.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3hhqtfyvf.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zygggwsz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3nflgyxsc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3jyfhmrfc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jypqqgut.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3arlanfhe.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jftjhddb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3cnfatewg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3abycnhqg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3orwloqmu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zgegrfaf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hiyxrtqw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3wdpjohiv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ubfidbyq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3pqangnbm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bbxpgwin.html


<!-- 参考信息 -->