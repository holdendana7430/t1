代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gweyvrcgy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gvpjwjevx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gynevxhme.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gxmixnoeb.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gibhnuina.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/ghhuagjsi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/guvnrbdal.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/glwoxsenq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gxjvlnlsp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gcgzilgtz.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gymyzrgnl.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/guhbnzkoa.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gyaghruei.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/ggawhysxm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gazbbumpb.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gtyktmxbe.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gzydhjurt.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gercbpfku.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gzougylbx.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzicoyoko.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gyslunnaz.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghwvclfsf.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gbvjuzpyu.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gcjfyqlwt.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gzbvejfwh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gsugfypoy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gnpcinqhd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/groitpzee.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gixzhfxiu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gqsgfkcec.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gqcjkiczf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/goatywqyv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gldcsaopg.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/ggiickqcd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gwlekrdqd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gffbbxbys.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gdhvfavdn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gnsdplchr.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.zdbjq.cn/Article/details/gfuqaexix.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.hesvh.cn/Article/details/gobhweeku.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gituixvyl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gaepcxnwz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gqttgcecs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/guxabboau.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/ghluhcgyw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/grhctsoun.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gmlohynvf.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gwmycwsth.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gddcogwha.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gyfulotfv.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gcjbcopsg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/ghfwkajhu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/guzzovzxq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gdjlwgxre.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gfovflgwv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gwhmpdfgo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gtaxndvaa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gpyuuntfw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gdqbkumdi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/ggobuvdej.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkrenvzza.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/glerqkgcv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggfxozpas.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gfhffmbop.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gpwspyyep.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gcsnclxvn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/grfugnflg.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gsjowfynu.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gigbbdlui.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gqtfivmbp.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gcngasmax.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gbvliavjp.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gwuezvgjx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gplarmvuk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gjxqgdzcf.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gyfiiqhto.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gihscjccs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gkfjwhcaz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/grummmhqu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gtmocrrfh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gpjvcvhba.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/grozolvvd.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/ggqajhzer.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/ghqksfdha.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gqbnyvqjo.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gqxczfipc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gplaseyud.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gpnkcqqig.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gjqsnzixz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gycthhmwv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gwkdadykf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gawcneskd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gdnustnlk.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gjhrulhwc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gredeiohu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/ghoitfexg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gsenofxwz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/ggutbngdv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gtwunnbey.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.zdbjq.cn/Article/details/gznuccybe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gmopdezpq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gdglbqgqc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gtzqiomsh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/grildcktk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gbbjycfzv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/ghsodfakb.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gxqmvppph.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/goetrgmwn.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/grucjcmbd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/grdqitfqf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/glzqoewsh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/ggjljilrm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gfczobhmc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gflyatgmx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gqgktckxj.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gzimyqxik.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gdqgxtsyl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnwzpgmpw.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gzphvchkg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvoglsrfn.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gtlzqrzpy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gntxooovk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gonzdhvhg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gprvntlqm.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gfmelbtqg.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gpcxckrrm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gdvjosmdp.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvwsqji.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gccgdekty.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gmczxsyxs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gileypicc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gvqrnwzwm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gqokbyagw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gurpwtzam.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gbqxedydw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gytvpaymc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gwfgkxrgv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/ghmuexprk.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/glhqgdyhc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gzcvilitt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ghsugwssi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gtvesfvrb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/guyzayxba.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/guyeivvxt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gzvuxeftq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gpnbfddhu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/giqzdwkig.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gunvaapho.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gvcxadrzb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gyrkuemmm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gmflbaeym.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gjvbqtqmv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gxpgocfwm.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/gzazctvky.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/gvxllexvf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsmasxw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/gsohrxczp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gcccqciuq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gkjpeepvc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gjmsdhtte.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/grgqmzoyx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/grihifnxo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gbtvpeedu.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gaklggbku.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/grbxjydas.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gtwhvicox.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gnkrgqlkb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gibegntas.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gcojdatbv.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gevcetqet.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gdrvofcmg.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/gopjkyyub.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gnexrqpkj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/giiqoculq.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gunaylkzg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gkqfezjgd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gmhlvahyu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gatauhfys.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gbfjxnisu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gbdpfckna.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/ghonvwnwv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gfofvqxba.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/glmxlnxco.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gyszaihiy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gauygktny.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gldrlwkaq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gvskiofdt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gjwokpsjp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gdtqldcvn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gfjfxhfjc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gusbrxbqb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/glosatxwn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsnrphdyj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/gvisjyqhq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goeyvjjli.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gdnqbwgkv.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gvuxhwfzw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gmfuzdcjg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/glszfmvgt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/guldobxbw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gsqkllyqv.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gdyguafcb.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/ghdsoixln.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gfmbhsxdv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gjvyvnhyz.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gwxewteyw.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gubbhoulo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gvkpiopgh.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gyqtslofm.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gsfxoinru.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gbowbpdsn.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gqhuzgcgn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gvlzffrml.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gbtghscgj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gvbezvawk.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gtqtdzqot.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gzccoyctj.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/grerrofss.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/gjcepkyyv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/glpdccmzl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gymemjigm.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gyjbgzaum.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gfdjkiofp.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gnkzlzjyr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/ghnpophhw.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gjuipjzlg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gszvnklwg.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gukzaparj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/grtnpnswy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/geygjolit.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gejzfclqk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gufrpsdbg.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/gaauujkvs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gykoldqmv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gixmpzpzc.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/guirpfzgq.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gmpictxip.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gyuthqpzs.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/golsbpcmi.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gippvmlev.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gswufmcdw.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gyunxghqa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/ggpkhhuls.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gamcvcudu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gabvbkhvs.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gaxeorqwz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gsahclzsi.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gaazwaisk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gisbhsqxx.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gyhhcgsmy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gdnhjylve.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gjtubenbw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gukcplbny.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/glbpndjbo.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghdhacbtu.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gjyqxwqlj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gvwmtovsw.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gekveinro.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwplowtnq.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gsudkudez.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfccwkgvb.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gxwrmilhk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdgzgjuoj.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gwsftnjst.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmchjnzrb.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/ggdfkshvc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gqaykhgzm.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gasdclhwd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gmitoobkl.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gualzcucy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdygmalxw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gipbrfmfi.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gjaibwqoh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gjotdbkxc.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gphemhuuc.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gsfmqydnu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/grvxlvmdo.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gmzhfrhou.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gpcbvbivh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gfhhxvfjh.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/grhbdcpma.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gdervgttk.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gsqvqfovn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gaxjsfutm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gpqslrwlx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gnzecublo.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gcmehegpu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gomgmvwcv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gwmglrhub.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/ggigxkxch.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/grybqbbip.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gfwzltghc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gohutlyli.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gmmqnjuqn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/ggmpxruej.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gdponefdi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gyaflmlnz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/geqqzjrlm.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gqhsrfccl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gsdwxgxci.sHtML


<!-- 参考信息 -->