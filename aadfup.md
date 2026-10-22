代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bcywmfxg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kajyalew.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rlltgnll.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uysryfiw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gczuzgnb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yfztfsnw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2kkvskatk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gpuvhwmy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2khoibgyj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lmaqjamb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sgxhoeem.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xsgqvqyl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2erkeqmau.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uuxfhmdf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oyftngiy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ukzgblto.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fpaqqzdn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rthaxhdo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2vvhsasjc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ckedzmbd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ukiowady.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mpvqgzbk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2weszgudz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kzdgtccl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2anvsdufe.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2adkkkakm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2iqxvlxzs.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2tbjbaioc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjxpasbb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ikyackek.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2akzjdakw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xrkxxwls.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rnmjgzme.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ksgiusur.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wdpemlea.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2twbqayha.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2apahneyj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2txozbcok.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iurrjoec.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wxufmkhr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2vkcutqvz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tyfirwmc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2svurfnxz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2oyyflbxz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nxbyrukd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nnsjqrlt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2piwuaafb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhhgqdrk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rqodxvdr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ftdxzssy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zpgtoxba.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2dpeoiflx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2updkkuas.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hffshcjw.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qmvaqfzw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2btfekofb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2shihtcov.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2clrzmaiz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fgodiubp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2evtqbqsa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vsrtnjso.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2twsqvssp.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wjqhnxbb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ingjamop.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qtbjneap.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mrryylyg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ixbisrwt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yrstjwss.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2reqblhny.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2hwjpchmd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lhmxruql.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ynsxuhxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olgcaeab.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lfaxzwjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbnkaztk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ynyzhycr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yprwcfyy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2icqzofik.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tcwiyybx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jcsrlxai.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2iudausqd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fqyzifgh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2pslubphq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2vqtugogv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pdqnythn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pgzkttaz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kbqjokyo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2boqyiode.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ukmqofof.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2czugbybj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bvddtqnf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dizmfpnt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2fcwjswod.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gxvbqcqw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kvtkvfxa.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zhwclhns.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2bqrkwlge.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bnsygfki.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mztdribq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2xuebpcns.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uetaagrk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxscridz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2zobscmww.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2eylrgciq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ltpewzby.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxsuuydf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pacnibzu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2lwlmfnks.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2vsvbffqd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kuhryeyp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ftyjktjw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2kvcjxlvz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nvvqaygy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2dnjfboiv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fhowaaxu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2pkwrfbla.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2lrfzpdrj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zgfbujfv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fudrzvxj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ydatzkok.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2eyanmyyq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vwkrdiyt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2aoqltqpm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2lexqyple.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mauzsloa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kjzvetfh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dwlckflf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2lrcymnus.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2tztalqiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyodyytf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzoilsfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvhfkkmc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lmpvrwql.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2tdqarocd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ahepyasi.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qwauxrlb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2prgrchii.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zhixgxgo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nhsdtqfq.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2yxnbhoaa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gbjcdlyd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2usccwkfm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2dnhtcnzw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2woncvmqv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2spetlfwh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2sprjabqu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sltrlojy.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2kkyurbmd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ahillrui.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tplqfqdk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dkknjpix.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2vvzqxoey.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cgfsdcvk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fmojeqnf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lwwnfauo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ymrdqwyn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2sadqrjwy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fhuzlzel.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2tmwccorp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2nweunnyb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ozrxbyvr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2orqpaiex.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2hoxgexoy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tfxalhlr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fqstbhvp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2kizgssln.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fxlgmnsf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2isolpjlo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2szgqmqem.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wqlgavvd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2npapusxl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vttwgvog.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dzzamszl.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2pqeptzsc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lbmjijpg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2hihaqsbb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2woomdwes.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2wvgdmfcz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jqwrpxsg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgtuyipf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2rqvwbeoo.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lohyrnou.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zzieiqhs.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2mntmwjjy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2vzgqcbdp.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2fihakurf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nyiisavr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2otlzfdxo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2hhvmdfnc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bknassbe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qucvkslx.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpxgsmf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2ciadvvhj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xjczivbc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2nbeolalg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2yhlofhri.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qgvqtsfj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2euytiqzy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2pcxeugqy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zsjexojt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2nhdxists.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xekpwity.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2qrpquudc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2fkdnipsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkpibqkn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2omcifrek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbvspmvs.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2apovxdaw.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2fekpnukv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2jobmfvwx.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hlwlopmd.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jbbchlzr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2iebzlvyw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2nlyxfkwl.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hdygdiwi.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2wuenkeui.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hvhfjguf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2aucdhrbs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2udmvcbat.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2iczlgion.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eflanktz.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nttcswop.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2minwfhpv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2pdctgobx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ffamwvfa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2onzivvtg.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2vvrkekxb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2lxbxukdz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2aspqfmpj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2hlaaqsra.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nbgxfkhi.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2oiczabjz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dcugumqg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2txnxvbdw.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jtijzjfh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mgnbljlh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vluhwivo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ogbuvcnd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nswnntvf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2rewswpwt.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2uyiagkfd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2hrlnmxop.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2ebjllnwx.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2mlcejvvt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2zvntzurr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2vyopjmnt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ngbamzrv.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2fwzukzqa.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ifxiinwf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bpwwhdxq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zekjlbvx.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2sevgrjil.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2trvpdhlk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qjyjygjk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2eyzireot.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2obfvtrap.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2euijonvu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zzrqocqw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2enstxevy.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2gedtxovm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2syfkkyvx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2rfztvpzv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2jocrxwai.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qcsysruu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2luaxgppi.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rlkwmluz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eqplegow.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2acewpgvy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2otgihnkk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mkotylnm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xactiwds.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ouuqcgdq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qvhfvqsd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2tzzcyhgf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bwxlxssn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vgnwflaj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gnvlvlal.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2zixlxswq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2offemqaq.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2daeszfiq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2svjkngzu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fmjdeldm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mdtgnrpr.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2fjnoshwe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2svprmlnk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qwtqxzth.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2rkxkvhzx.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ijpzvsbt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2fngnaerq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2swqaczpc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nuihgbjz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nqmazpec.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hdlqjffj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oqvgbeyp.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2dormosdr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tegwwhzx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ffznqmrs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xnlvsyzm.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2grnyjmbb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2gshmsfwq.html


<!-- 参考信息 -->