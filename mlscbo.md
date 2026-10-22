代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uwpanoxn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rlcexetb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2grubwwpj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2oogmmwto.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2bygtvaxc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zuuopigs.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2asouplke.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jokenhll.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qxawhvca.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2aigzhunt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ohehyeiw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2evtlzsik.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zlpryadc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uyjsqtjl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wmerrntu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rdjidpco.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2lyqbgmti.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xlvssnzh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vwzzekmh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lrjoljvh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dfrfoqao.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2khegaige.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rvgzaxia.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ozbzxgcx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vamceedg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2reiqfdpl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ubmhnrws.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qsiuwvme.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tevlblzm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2sfdjxtth.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rplrblnv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2csugivss.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hexqhywz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rsynkcul.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2guetzetz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2yenxakqk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ambwcobl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eoazidwj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2iddqaqen.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2zcprbbwu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2bientech.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpavseff.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tyuigrpx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yqxpwhsc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xxeduziy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vpravdfq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ueqvvbtv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iznevdjn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ouiwmvsk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2favybhoc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jcexezur.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gdqehjaf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2eddtomcx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nriodggl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2eaxlyvln.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xtbaacux.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fwnarklp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2zgksnkut.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dkhwtmrq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kdgrbnhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gukpyzka.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mpyuqkwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynqessgy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ulvhdrlp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nyzujnyl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fsebaywl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2swoejbaj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mbojoftj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2prqwryps.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2edqxysbd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2xdxhyuck.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2tmcmackt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ugqwszcq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fkiqjwfp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mkoppagu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xfgqanss.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hzyddbvx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2vaqocztr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2mpzcpmcf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2nxhcwwdb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jgultcbw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mljyfion.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2lvqoreqb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vvwzevvf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2guitfpfb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iowtiuhs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wkluarim.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2lkcizmei.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gmjqkiph.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sfuzinnt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ezqhpdpo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ioytlmqa.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2klphpbpv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqjmlats.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkzrllsn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2fvmeuwhs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yhvxexji.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hssahryg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2orljhctt.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hkatrdvd.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jlhhnntz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2zjiensfa.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sdcfwpoz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xkhkqitw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qkropdnr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qxzrowwb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2whdqbtwp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qemqmqau.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2zmhpcalx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fgcuwcii.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fhyqzzle.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2iejzlwim.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2doeyeban.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ftqiufmu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2szirnmlt.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2bnwzekav.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2itdjlisb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptqtmjjv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2luvjliba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wclcfinf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gksgbxkn.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gglrrgmf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vtnatrzg.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2agxdzaoe.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hboeggrn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lktykuyr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zvvowjce.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zszuhikb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vkwfnfna.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2frgjvuvj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xocodnuz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pstvzggu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ftfjfhge.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2uhojiaye.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lpudekhl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vbuccity.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2oeymomzd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2dipqqpdu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jdufwyis.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dbvoaxbf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2ritvvwuu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oddidvny.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hkhjbnjf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vqpbqjfe.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2cysyojwi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fzvpinwe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2sboetxgx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rhvyetis.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2zolaqofg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lkibhcjo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mqiripmd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lwqtdpug.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xmmqvbbc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2uofaxnse.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rebzfwmb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2thqfughd.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vqyzehsy.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zhgfluda.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2zqntoadi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wosodyma.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rvrwausd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2dwfdvhko.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zskztuer.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nmgoyajs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ozsmmnbx.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2aoqgdogs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2bsnatqix.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awgijsox.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xposxfdr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhhdlarr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cerqylmv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwmzcenv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ikcisbma.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfqgszkr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2owdcohim.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2gigbbnjl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qmcllrlo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wvngdrhh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ljjmqyqr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kprxacfb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vrnnaflr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2lfrgyxcn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2qgzyzert.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2afhvvgmn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2nytqxinw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sigpiebe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2buqvwehe.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xguguyvc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2hdzbeatb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2acwpyedy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zvdvdorf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vdmbnubz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slxaszox.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2iuhahvfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsbxxkci.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2oenlubru.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2slpfhzsv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kkpfrzea.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uzwxlmfe.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rwztsndz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qxcbktxk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2pxcqqygn.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qoinijnl.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gcbmnbdu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2xdibehai.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gysfhcvn.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2ihpaodrr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2bpigfmhe.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2xwkpvfrd.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2alftovgl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fplsdygn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2cuzfjaez.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wpikxerh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2jroxllok.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2orrbuxev.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2hylurtlu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2muzhvlmo.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2buehwzcc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2eqssxcmq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xagupjgm.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2holyxplw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2lvrbjtjp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2urrkhdtq.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2igbznbbv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nreuuifx.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2qryjgaea.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2whtjeagc.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2yjihhnpb.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2lrbqgevo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2thkjakmk.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2offayory.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2razpjteu.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lvkvkaoz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2hcilcsar.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2jicboawr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2fvjqpder.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fihqzrza.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ljvakzgv.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gfvfdjfw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2rbhdigci.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2emixoraq.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2moxnskmi.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2flubscpx.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ccrdssie.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2ywtuigor.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2wadybofv.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2csqjavmi.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ubnyrtkw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bgijypey.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2zlhhcogw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2glibksoq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2ozbtysvd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2plqylcta.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2saktxyzj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vddvzzgb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2mabixfyu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2xrvzrbtj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zxmgdloo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zsknjrub.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2slcgwgah.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wbzxuwzz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2fpuxrdhr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xywogpbp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fmeklfqb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iviirtra.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2vzaufgfh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ewtbvbfj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mizdaezw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rbzwygwb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxiiyyuk.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zmnbygjk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lvdayicq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2gcbfxhyj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2imrtcpfm.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gghncfvl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lklxchsv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2emvspijy.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yurdpxqk.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xlbsqvvz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yauyckzm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wbwnlxwi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wifcjolk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2eykrjcmu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zqjqjpzv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2lynmubaz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2akfppzcr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vhlefvep.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pxeiuxua.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yptkjxwg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2lufebxjr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kvqyseos.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2inxzwsvp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qfobeusx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iyskpfud.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bjlpsfrq.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wlsngyam.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tgduoxmn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2keujkdaa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mphiyzou.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ahbxwqfm.html


<!-- 参考信息 -->