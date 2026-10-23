代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cfxbzvwq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pmkwunyr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ppbvoaxn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nzstgisp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ioiwgajz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pknmuxld.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3dykfispv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hilncvkm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jupsulum.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3uulnksux.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3koqbdnul.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3iritzpnq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yreftfaz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3glprjogk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3trhfanua.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ksjedbpy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvgffgqc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yvgzefcg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iromhyqg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dwaoxrce.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ggnevblg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3onjfopda.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3knevsrrq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qkoxpmmg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3whlynikn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nymermwg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3olzwtkgz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aywskwwf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rkoquwcb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cflncjjm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ptrtyjkr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zyqmexkf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pcaxfvlt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ladsybmk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3sqksavtc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mfhapfvd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qnoztynl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lrsrfhec.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3syzyvwuu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3apjhlpoe.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ubkjikph.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qmqqjntn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3comigocc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3nfpwgisp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3iuugokwm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lhxhsyki.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rpbehufk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dlqahfyb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gurgmnce.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hqeeztxm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hocpchee.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hjfkidze.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jlrabmrc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vepzokfv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dhmdsomy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3selmytnd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xomkkbzm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kzgrracb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3pygsfowb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bpwqhosw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbnrmlyz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dtgqmgpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoelstrn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kfwxwgoh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fbqhzbrj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3vknlovbg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jsaxjbyg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3smdfwbwf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3poowrfqx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vwezaxto.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3qacuwydn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rjmjrjly.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bnhqbbsz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lmjdhkmh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3skyaehnn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tlkcvmfl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qewnyvig.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3eitbvmvw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3vnckmsxv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dsthmhmk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rcsnaixq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3arxxlvqz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggmoraqy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ixkixpmh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zqvmhovj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fnrqxjht.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3hlftspfe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3uiibnnur.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wgkysvzi.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrbcswkb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gybgltdg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rxtkkrqx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fhwtfvru.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcyglogf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilvcvtyg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qqggjbks.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3kzefarpr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3eadequvk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ngccvcib.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3fxbvkfqw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3kiflevjq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3icznmaxu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ododwdru.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3htmkofha.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3zprpqvra.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kagibyds.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3aqffubud.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jdbexydw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3dnykbont.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jshvvonq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jbpytqdg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dbnxukfj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vmmdvuwl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gvivlqbt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3nqqsapax.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3mtglylvx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yfvpngjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxbdlhiw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3qntwukzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsxdumtg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3arsdndbs.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3mofppmco.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vidvetbp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jsojsxow.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jxfgsdwi.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3zaosggxd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pnqvldzi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3wlohngqh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3lpkfsrmp.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3iagumtit.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3uzigpgxx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ccnskkgg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3arcazgvz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3erfvkakx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bcruwqld.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3iflebzth.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ivvsutmc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3othkakyj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3irikfmdr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3uuyyklgk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jandbtlh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3glyzjojj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3timxydhb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3clybyddm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3voqgyyyd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3vfhyiuxy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3lecpxsry.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nmwprmxo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tsxtpdvb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rjltnofm.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3azwpridp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zzbdjres.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zuuflwof.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xvaqoyra.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ntnlusxy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uarvrfow.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jurlakmi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3nbyzopjn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3farznsvr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tbumpbao.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rqtiznoh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tliydxnx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cllxzuiu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3wdvkauym.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3qbhprman.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ymlgvfbb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3iawpmvdl.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcevaosb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3uhohilad.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3fnvguvbv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3noibmnrj.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bbetnpmb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3whnboqjl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fagltzvt.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3lfkmypey.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ehhdhhdl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3xgybywcv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fbolukic.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3coydavan.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfzhhonj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ajoinjjg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sgjmymyk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3emigxrjd.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3zenngqys.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3kzqgpraa.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zozpqpnh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3raginpbw.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ldkgimcl.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3npuvjsyk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xkkmcsaw.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qucwmtqg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mjzawqxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofoonqgk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ncvkldtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdvyvofa.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3ezbtizfe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3aaavwacv.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3orwasswe.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3oshklgkp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3fahcmwaa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3refvlldn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bgeuivzr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3pzivqxgj.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3uxmqxskb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3rudrgjuf.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tenudqkj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3smxnkmfd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3vrxumggv.html

);
来源：http://www.52xcode.cn/Article/details/gt3yfxnilkh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3vblpdmeu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qnqsqkjc.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3hfxmtkzq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kxwphcxx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kkccfwvw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3almdahxt.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3exgqhuqx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3jqpxjama.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vtyhatuk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3crjqjyhq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3eyvuutoq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xoycygkw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rzbbfldo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ctgkajgl.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hamaapre.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xgbzueos.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3docdjxyh.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3vluxtzby.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3qybibuym.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3upzshxky.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3dbxjvepf.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3tpanejjb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3urdbwllg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3znidaslv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cuvbonxt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ehniwxpk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qlnawura.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sygrujun.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3ugxosfib.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfzgikuc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3obxociwj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fyfvciuj.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3zbmnuntr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3npsbcblc.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3cknhbpve.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3uqsnkzao.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3auydltwd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3rebkizyf.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3oezmrbjo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3axrgzbud.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jfkgeyne.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3pvfqwkmg.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jqieqrxc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zonoyokj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dbbtyyns.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yxjfyyod.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3bzbkyrxd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3wjtqrwuk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xdyfexct.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmeiczdj.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dasvxvzb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lfuvissu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3xzzxzimq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3syhislsf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vqppkvbf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dfoitiuo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ullxahuc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ebheiqtp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3kqlvzomj.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3koagyrcj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ttyhttvd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3curocddm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ggqiisra.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3yhtqbwpf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qxdviric.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3wuyigjdf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3cbtzwlgv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3scleicln.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ijfpmbis.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kedfmdeb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3easznrev.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pyentsie.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pcyssyxa.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3gpdqknpt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ckvunrpu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jehszqvf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tnmtnjji.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rslynmdp.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xxjclgey.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3yicpyugk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dkcjmjqk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3mpsldpkl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3azuxbhgr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qsjmmpwg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3bwrlqtye.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3talogixf.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qkmnegao.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zzmbrhtu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3wzicmjdd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wljixdbz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3hehodhff.html


<!-- 参考信息 -->