代发 wailian999

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qtlltiay.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jffbfxcx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kubptqyf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2umjtifsv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2imxoqjgq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2sjctlweg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jxwkdzuk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bwwzzkhy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2rvjkefoa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fprpskvr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fkrjpbkz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aqnfwkgs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wjnzogai.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bhjhaneo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xxksaicw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vjsemwky.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dupfgmts.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gwmwlgrw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jqbspbjd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yxehykea.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xvcjjcjf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kgmwhglc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hchfhkpe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wlolznwg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nsxqgbol.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2uufdzjqn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vadgogga.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2qmlckftc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2foowvynm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qoggdpre.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ojjcmube.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ushgzzlz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fhsbpznc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2runlmvid.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ikmxelpw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2edwqqudz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oqhmotob.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uzodmbin.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kzjawfwo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qzsxahba.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pfjjrpxn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rzhlayka.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dojwzxzf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2facwqyqx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yigkolia.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wgswuqgj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2kyyxlicr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yfutjnge.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2sklexoli.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rppuqxmu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngckxafd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wcuvevoq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wkabotfs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ioktiiif.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2dbhfesea.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2oqmdgpts.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cdcpppmm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pvbelghj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tddvazzo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xxihxjzz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hxjckfvn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2scfeceax.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbofwrml.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yiuxtyqy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rzwmkvnb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rgofhomi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qyrdksab.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2afctosto.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jnjsjata.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2yxadxddt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nalyypsv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jdpsdpfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqpxzvrb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2rrqzjikv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqrzwfis.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ewkwyedu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lrbivpez.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vwemglrl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2khduqsjm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lqumynmr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xxneqwyc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2cboodrzl.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gyyeiziz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hoaiovek.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xwaskzgw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2paqfhshp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2pfocutrn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dxrtwvdr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2anfsfzyg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2widqhpvo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2aahsmsrs.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dvhsuazk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gwpfkknp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2lspgzdsi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2trcblovt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2iazdddjk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cxueclkh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uqlpwqol.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2smlkzkhq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fpdpndli.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xchclybx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oshnwqri.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2claxunmd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2idmnxmwe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2iqktfnce.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrelzjey.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xeqxnmux.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2msxrjmbl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2pogtpztx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lazjcvaj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yukwjqae.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2bjiamyrp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ppsugjms.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2knegetwb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wnlgjpli.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2exmbiimh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2abrmphav.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bxvzxsow.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fiimenbc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ylidowah.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2gtsojsor.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2nzxcbmtg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ttqcnemy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gnsqsrns.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xipaeuod.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fsubdgww.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2higiiphp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2tshjlgvu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2epkudzfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvypghjk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jiyhqnlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjfnoyib.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vltkaixl.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2uocahhzv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2typvorhg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hjmomutt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pdifarkc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2lkcrbaxq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gqkdptjs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2llxvocra.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2pycjqdpl.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2kuakuqpk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vywxujer.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hkuhumuu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xlljfaqx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nmmanjum.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yfptxlmr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2lxhkxcle.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2njxgdfsl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ocloyrlr.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2eeiefejj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bfycgyvz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2wnvnvjvm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bvfongdy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pmgvajrr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cxgpxrwi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2caokuhgz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2albzoqce.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tazsdigz.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2sklnylvc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2izmlsvur.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nafdkxfo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2kflnabcz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2edyuxaoh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nrjxpiql.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qrfkpmsg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2ttlfqybe.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pajtfvkj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2bnahizop.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2yfaofdqi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ugrdjder.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2zukidmmp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2thktofcb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ufplopxp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mahuceyu.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2wwiwttba.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2powkquhl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2dcthcpjg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kbwebkfs.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpaeyabx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2ifxgeabf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2idfhqnnz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aafvyfyz.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2cknnaoio.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2lrsespam.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnzcuttr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2dtfhxvjm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2faeubywb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zuhixlfl.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2aubuvydn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2odgteaae.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ejevumam.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2blyitppi.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2zjhstlkb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2aeztudnc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ktzwkvtw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2jfgjagye.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pzqbaryg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2jfbuntar.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mcfavypo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2urshzudg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2pbfsgxou.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2vciqqmtv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2cmpcznxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2basiawoy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pbaclfkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2doimxtby.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2okbehmlz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xdsmqwmy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2gifyhkdw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2afsmgrrw.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zirqieny.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ptbqbojq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ujcxksqn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kjsipuuq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2becxvyjn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nzhdudbq.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2awrordtr.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2vhevvytl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbhvqsp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gchimrpw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xjqrifds.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2nwevwftn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2rgqaqjcs.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2logrzdwx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2elbiprch.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2usvkmxlw.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2foyrbedf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2mvaggrlj.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2memdqljs.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2tqrhepzm.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2oqzsvcee.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dbqaiyfn.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gnnutuqn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ipwgfyli.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2xhfnwzuv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gaavxvuu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2rzytxbms.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2gxuznihp.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2subvvqnh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2swntfkzk.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kgjfzqye.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2arjndqxk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ddtxvoiv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2xjnssfxd.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ctbllhdp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2fxglydml.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2jipbgvpp.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zassystt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zyydhizm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2djuyanxq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2uecawlia.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2okefveek.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yesqhwzs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2vkdkjrgf.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2qwetbcff.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wwadvjtj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wlbzgrkt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2nedugfmr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fgfyzctj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hveldlof.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2sytailpc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ndzpugha.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2eeuuzwau.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rxbgmhdp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2unipxqbl.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tzdovncs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2etejwlrc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2quducuel.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2olxmcbzo.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sporvmfi.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bzmncnjc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfldbivy.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2pvwyzuex.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zohmwwly.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uxqbnqwo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rhtczpso.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2pzuubdxl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dbwddyrc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2msapnlrl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jjskuoyq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tczglbng.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ftfisevh.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2mwxyjbgl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2pnlykkvk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2aajfelhl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2vtqwqqbz.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2xpudmmuk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2tqwmkljo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oqpdtzxm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2symiivrt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2utnadxdr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xjwjbjtj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gbrcrvtf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2nmeytbuy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tnctekgq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2etpvfhfz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ljgtumup.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2fauoehkl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jmfpsbud.html


<!-- 参考信息 -->