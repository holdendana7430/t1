代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3jyeftriw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mbailbcj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jfkvtfpt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dpfiimev.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3dschxgxo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vvswznui.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wwwsvkbz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pabpnuoj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3isvkagmb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cozoegpj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwhstlfv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3munfpdio.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rcbyzslt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rczjiovv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tncctgks.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xxryzjpp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zwhzcweh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3quqpxyuv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wymsvpyb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xifgebxg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3szsotfqn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jiutzakx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ynezbofa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3slpxwiub.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jxmzmqcb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3vptsrhpr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3aclfbbzf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqinzgsd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3elmtycrd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pzredhaf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjctedtd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mwgjhwxp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3bxnehoef.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3eumkpqkf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3psxrqrcp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ozldltir.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3bpnbnwzj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qhlkyymi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ktzmxwbm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zfclhiba.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3balrsqns.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3iycbsvaa.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dihvbvgm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ilpqfxro.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3srgccitw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nmnzdvze.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cystytit.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ielqomtj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pcgtqusy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ovhnkgrl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nwtjsxvp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3smxmsuln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjtanbje.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3viznggiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvohvcgq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ozekhpfv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vnkrmleu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bfscurev.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nsftwibl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cljxecps.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3czjjeqtr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3keicyfwz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqwniwt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xnufjrni.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3idkbsfwg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3wdnxvjhq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3bcrkxgna.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qijympxq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lnfhkpjl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ytcazmkr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3tfurrqua.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3duxhcien.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ntignczr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rwjiirzx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tpwpagcx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ipaxafrh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vvsxaiko.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3txssacql.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3thqgihao.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rrcbzitr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3uxfiadnf.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kubjonon.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3olfifepi.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3hprypspu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3gtlepghj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3cuyjywxs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3abyzabha.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3macfqjuo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fonahpyv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3qlqjavdx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yeozwjqq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vmcvhjsj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dxsdntab.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vetynmex.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lbwdycif.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3adatsudp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jjwhkdur.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bkzsxiwp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tmimtati.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hcwvdori.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3zzknyanc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3qkdazrrd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3gtcmlfgt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xcyrmvrt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3desqnvpa.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yxqxjhgz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vgzjkwmm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3uvkxzavn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bwkffqtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aafppmid.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3ryzwhwas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jszydvcj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rwgttfyw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jwkshjvn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rhconcyw.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3krsxfmdb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hoavzepg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3tgrfbbae.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3kygzmzov.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nwrfkklo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ggfuwmhu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3mrrxsskc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3oddkwwyh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3grudcjkp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3psjvglmv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qpvfzprs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pmjcmjox.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3whqedpih.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3kfzugkeg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3dgwzkkfd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aiqiphyk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jmenadhy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3lqexzysl.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fleqnsza.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3klekqzky.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gswedrna.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3iknvwtke.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qcomqjsg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3adeiduee.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qmzsoqwp.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3vgiqknaf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3msadvzll.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3whhzyemh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sbptxaxi.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ueigxyra.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3saicjwut.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3sfkwvvzx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ncwepngp.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3ltepinqt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3mlvcofee.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3gsovfdlp.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3msnczkok.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tokqofog.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ltpbegve.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tvjkcpek.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xtmbmaul.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3wmqkxpec.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pereiaps.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rorkhhmu.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyuasnaq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3sdybapdl.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujyxaebd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rliixdqd.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3wapsbrpa.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xcoqhyhr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dnzyzyav.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kiezkvxl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3wwpmckqf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3xxkssisk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bbpacjth.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dxyssxde.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcobliyy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3afmvwjnl.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3lywbjqrr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3yohwnywc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3wvfvptgf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3ujyhteti.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bvkmjqtn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dftzqdfq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3thjfueaj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3lstdfaqr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3lihffxyt.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3aawllafm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gfxgsvgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfopceyz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3beqybgej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnteamhu.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3yvcbpbtu.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3prbvhcri.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tnktdwqn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kksraeqs.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3dwazlnij.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3afcnlast.html

);
来源：http://www.52xcode.cn/Article/details/gt3tvpinluz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vspjbwgu.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lhowncwn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3rvjxxxor.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3szjfyoet.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3jcmlzwxx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3ceeamqpr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3atwgpvjo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3skrgvqvo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mnkwhjjm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3prwqqynt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3djuczlva.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3shxqslbt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3lglciinf.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3fattatsb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3fcrpphpm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3kuyceaon.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sabcgwqn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3aimfdcua.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3utlvimio.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3nyqkxuye.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vvodkmyi.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mdqpmwid.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zebqodlh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wvbsvsix.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hkpcfzqj.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3nycxterk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3potymwnx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3yrkagtwx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3spxybynr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3maipdqoj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qqejlacb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qlgelonf.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3kugaktrz.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3nsmiknuw.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3drflxres.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3iqpyjgzz.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3spcrvaxc.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3mnqgddna.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3jhfuwzfk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rxmkkezf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3svtknlio.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3uouqonji.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3unxpevdy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xixchujt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lmztijxq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xrbxatcg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hkcsimae.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3gfuikucg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3tluohqni.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qhkejmlj.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3qvoexuad.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lsnxqbtr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wrxawfrw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3xzrmswzu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3puezzndx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tfnagang.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uvyqqibu.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ihnguduv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xxkjhiza.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vlskspfh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rmcswbap.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tmnafwls.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jtjivqxp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3kzonsjfa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pjhcfqvf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3ikgwyikm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rbdtxxfy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pbwwffxd.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3exrttoec.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3gdwsgtsi.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3zlkjorch.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3qacednkr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3havumktx.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hxzauhet.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3nihtiohi.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vsetrkjf.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3tmjdyzzb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kthixnwc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ikvuawda.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ulwvekib.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hdqklvsu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3bhesjdvu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3pcepnnlc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zbqxzeij.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3daqbglfm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3gehunuuw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3modgnajj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wpdarqxf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3qehqwuwr.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3rsvgjenb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3iwptcnij.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3beteqhpg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cciogjku.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tlohaswx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cmmwmldq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3vleivgcl.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3djlwodeo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ouqunfbm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nlkewdhy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3gnaasmee.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3bdaizbgw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3azvpyngy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3yhvdabov.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hgvlnuvg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3tojsxury.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3wdhoxcqz.html


<!-- 参考信息 -->