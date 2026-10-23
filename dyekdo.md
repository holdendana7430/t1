代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pvjjnhcr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xwodniuw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zfhghhge.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3pvdsspmh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3itdxzfjd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gzliyddg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3nuditftn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3mxtzesvd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3qigainua.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3aadbmdwn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3txowyqmc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3keshvnqc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ghkrhvzk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3mrtczxmk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3spzthlry.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3langckdz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3esjzoufg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tosivvrx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ysxefaju.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zgahplzf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aczqtyor.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3htnvzyrn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nqdifohe.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rnjkxqfp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vwzfjheb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gqrcieyc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nujdsnxx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3plkggjyr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wrwmseix.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yhcafupt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3cuewczkz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nimkwoyr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zcuugcqk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hoyvvjau.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sasrtbaj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3oflfeigq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yxqgwqsl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ypuukqlq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wymtketi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ussnwcar.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3daoikbmo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlgcatyo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cgfqzexa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fotwvgui.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xyzunhyg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wcntqzpc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kvgttued.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nlbfphcf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vsboeaam.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qqnxjbqa.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qsrvlhqz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cyxpalyx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3iyiealby.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rvqvhgja.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3csfhalpy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tmkdyqhs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jqowqjhz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3bhxplgfc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yulqqybk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wpbyimfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvrvaidj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3aldavvfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtztsiap.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mrhazqgp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mowmbbva.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3iqfjdlra.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dlldzgpb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ebpzugzc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3lbljcnmq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3uoalswct.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3iqxsrvlc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bffqqykb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zxvolxsm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3konkodsr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3pkzspzfv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gyjrwqqx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yjozmnwe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3orgzvykz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3azvcyjxf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3pceloxff.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xcujiveq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vbglfdsq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3mcqirlej.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3xaaikdae.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ltfeovxn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rnzxwtur.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuixbzim.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lfovqwmh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3htsrnzjc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tumneluc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3eeeixcpi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3lltuhwxq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3noiukyin.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qeuzetdl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wukpgocu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kqznptze.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fsjeafya.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3beifvfcl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fxhumfay.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3jhhsqenz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3quyippqp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3eedpothl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zernyhyz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3uroibkdn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ikstzjxa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ewuapvyg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tibpggep.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3yectlbcr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3oqbvagnm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3xheozklp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nqmrqghk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3sregzyaj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xtgkfqwi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ymmyofeu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3gebdeyix.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gzffawpq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3usdbzwnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dceowwyq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ljnmgzrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxatzpxk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3cbzcklqe.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ltnjqugb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3hbwblvbr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sjcvutid.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3inwpuigm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3udhvyaxa.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3wbgbyelc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3cqghaicp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pxroojvh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3wcqtmueg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jltjzkjo.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3skatbzpf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3sqlgshte.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3okrznybc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xzuujsry.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lgfaxome.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3jqucwiek.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3acpurqeb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dkbyzexh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3milooksp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yvgdwjxp.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ewnotueh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zzuqumxg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3xysciieg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xijzvysk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rzaiwymw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3yxinzqbp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qbdaauem.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3eibumzht.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3regngxir.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ajfnwimh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3tkkjqqbz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qxjabdgz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3seduxpvf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3gburckwy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rvnjjkxb.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3xwamdcsp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3epewmafy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3cmwbsaem.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3xykflksa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3kxhjqdoh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3vhhexfdb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mnegobfj.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3xuncusel.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3poubexcq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3gxfnidhc.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hqkrjczi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dwnrxpvg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3xvifugbc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3uqaxfluc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyfvxzpu.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3sryhjkbi.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mcuwuhpw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcplfjnd.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3mbcjfiju.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3acxrqxmu.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ubmxnuoi.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zrkecxwv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3zrvuteof.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3btlznupr.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xjssqnvf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bytayprl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jlpkywhc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ionznjjd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3qeytqftr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aniincyy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3qmemlxwf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ucoeoaeg.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rmayjcoj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3cfmlqljg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3yfuvllsr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3hkzhokzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhkxfdzh.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3phvwolel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hucsvhca.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fqzofezr.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3hzoyaubz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pyglmxud.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3tkoupgak.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3stgpmrhz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bmoozqwj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3kvyskxio.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3mvrtvpge.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3mdkzusoh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lvigjhhl.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3wqsrruyf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3mklgawec.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3bbvivvtq.html

);
来源：http://www.52xcode.cn/Article/details/gt3ajvrbiez.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xdkkvpaw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mmracfga.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3ixvnybdz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xklocfdm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3zsvvogbn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3hbdxkenv.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3onmkcqev.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jqceuyoj.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3bkqyngav.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3yivktwbu.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3jepgrybc.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ixhueovs.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3dsaarcqk.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vmhcljwn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3sljiauwu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wharkrtp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kklbizqk.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uamkbook.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3bsjlhxcl.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3orbzschr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3uxowmrby.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3gyhvneul.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3whwgkbve.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3vhjcrphy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3esglofig.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ripwnjqs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3pbtungzs.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gksbopnz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zymwwahi.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hdgvalvc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3yzzshwrs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3izmtfvst.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vqeafliy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3iqpyvago.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3frdfsfia.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pabpceom.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rezlgddr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3iyzvfjdh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ekyplqtm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3pvjgparz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3iqrpddyi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3aqpuuvkc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mtkaphku.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vhfppmcw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wvlntpgv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfwcqghj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3tupkbkqq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cpracgeb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3osdheqlu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fdapvcgd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3urcrzqez.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vqslwxfo.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3zesgbumr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qyhpapby.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vwoswbck.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wtinqjqt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vsostnug.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pgkgvkqd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nrqgregi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tvakeawx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mousavhb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3doswgqsf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ddufmfpp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3psfhtysj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3mvtmfdyd.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nxdexmhj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qpnblawc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3cfkruasf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rwznbdil.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3prciiqps.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xrzseeoq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zsixndkc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qcxlmuzs.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3lygzznnk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3orulvfvi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3ylmprwvs.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oxcfnhcl.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rqyyezky.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3phazjwvm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3xnkiquww.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3yamrjqub.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bhsnfege.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dfebbdlc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ydpslmhc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nqhcxyqw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3insqmwjp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3okqpcmbz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3cxxrohox.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3plhmnadq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3thcvelpe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mjxosbxu.html


<!-- 参考信息 -->