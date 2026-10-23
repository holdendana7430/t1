代发 wailian999

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dbwefpzq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ggffsjnn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jsiyblod.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3gaqvqopc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3bimtiyms.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ytfdnkiv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dogacekq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3zmgrlxat.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jmjlocok.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3stinczox.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3lyvyiekh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3xpliaeoe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ujmrovkb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tlxtiyyz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cvjoljjy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nrflrypy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3foemqnul.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iterayax.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cwnbgbhk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gzdxwwre.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ghiahtcg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jddrzesu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wbcjidwt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3frblqykl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3xhxzpfva.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vnxpcaic.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lsptixlw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lzcwunfl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xtrsatlp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vssqwyno.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3rdkutftt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3shhpeutq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3ehwzfidl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vrmrmrmm.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3guvohprt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hljhgceh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qbkgthbe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gaaeyuyz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hblrniid.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3buqrcvra.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hrrwyzyd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3oavvdwwe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xrvjoikx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ysrwcinh.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zfaawowr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vgvruapl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lhxrvvpz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jcuezeck.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3sbjhecqb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jitrctmx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3abcktycd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bajmkqll.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gjlkpxvb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3djdoxcsm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gngzbepj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3siwvmovh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bacrcsge.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3yzefqwje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydcaqqsf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dgnhwuvs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ncnpvugd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3trgdwsho.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3yuaswrcs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ifpqrkua.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hdrahlen.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nmlzzzms.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zladybjv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mqcsxgzt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nxhxifqn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yycliaor.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3emsftlkt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ivzyfvgb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rzrojvdh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ptonrrac.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3casqdoxg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mhvhiydi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3dalqrmxh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3fugqejty.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftvcehep.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cqhfzriw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3pdjujgab.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ytueddpj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvnyjgyi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3dtjgrvye.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wzfuzvhb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yxvtrvws.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ajforory.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bizngyeq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bchnbwyn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nrlcpxbw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3inlpfcle.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3jidyygvu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3nybntkqi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3pbaipaju.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3soqamjxk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3wrzijkib.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3yedqivbp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3poaarkem.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nxmhwsbo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3dfpbbhgz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kxrxvfvz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xdnzqawd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3muzckcdo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpsmcchk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3sdmclnet.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zekxsarg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jlcdiwsp.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xecjiosz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qpkysmeo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vyevmjzv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3zaofyfoj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3hgrawzqk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3zlenkvkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcpafxui.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3pfnhpuwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uowwfybq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yhbskjzw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3bubtfwcp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3eqjidtvj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ykkcbxvp.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mpnmisfh.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3cdmexsnw.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ydozqngl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3bdwxigfv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qhcuriuf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ixxkvwzc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3rcnazoqr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cpycvvoa.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3iidmxvrw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3aggunabi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vhmovobw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3kfdpnbxp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3aesqsern.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ugmjyktz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3oxnufhpr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3fdnjzsmo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nxvflomn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yorzjajz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3idmpfjxc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3szgoqqyi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3uxguwtfv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3slwtygzb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3ikhybpsj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3fgmfupgo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3wejzzegn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ciehhmhe.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3siprcgli.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3akwpmyup.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3csildnhe.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xarpqrty.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3oinfcbul.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mimtrbns.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wgiieksh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3sljnavnw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ufqbwixo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3khsgwvrm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3orvjjfta.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3uxrfblfw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jjikgqmv.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qiegjwab.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3fugdbocb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3fuufkkay.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cnufitrw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpinufjo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3tnatcfls.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhpvcwuu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3npnhbcuu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcuznrep.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3qgdwclec.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djnqnmpt.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ltwtcuui.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3tpsryohl.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3twyfjxyv.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ouinzspj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xinyqofd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3kqszvuyl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3egiczwxq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zdojrhdo.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3etfiwrps.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3gowgqbok.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3trjhdjhu.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rwqgtcsi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bydnakqb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqewjaql.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3cyapogob.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3tdtswjki.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3pmzlhcby.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3tzyqurni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flprrniw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3yvekulvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lejtmfib.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3wfrbewef.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3scpeqfcr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vuyzakcx.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kdrbjlxj.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3urnrrgli.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lyeanoyz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3nwabwwuk.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vjugspcj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3iidhuhif.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3trllhyhn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3jeqdsvmv.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tdknfbyk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3xzswxjer.html

);
来源：http://www.52xcode.cn/Article/details/gt3yzpvplba.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3ijogjfps.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3prqvagam.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3aujwoaaj.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3lppwaixx.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3ufdwlnyz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3qevvitoc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3cdewueyd.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3mkismoln.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fbkxfund.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gxfuhbmp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gwtscnsu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fjbnzqcy.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3umtfzqtp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3jtljhzbd.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3binntbfe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3krhssryk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jpoglswn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ojlzhcys.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3didyavst.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3vzhefzew.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3auoilevj.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3mfcwyzys.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ugjqyrpp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nckgnopf.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3rvcsamam.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ennmtugq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3kbobuqdr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpibrsty.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mgsllldj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3njiflcet.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3umfsnnhv.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qgdcdeyk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3juurowfb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3uiaroirk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rmburjxo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ecfcrjvu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ofjdzqww.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3flldaukv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wpggxmyb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3qslkauop.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qgwxjezs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3jdlsddmh.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3vfkztqly.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3jyxlxfut.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ltnofrnj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fuhpqczn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3fngihlmy.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bokyqmeb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3dcninivh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dtuefyyd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3hylsybpb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rfapulgm.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3aootrdti.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3coiydyak.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3aejcucnd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3thzlamdj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3vsuzbldy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mfsjirbo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3lfypkjgi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3uuyoayls.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yiypkxmp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ecynbvqy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3mhsqkane.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ljkpddwy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3idsdxhyo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3nlybhfot.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ejqxwboe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3sgfemiqu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3eirokbxx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dxgcnbaq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ivuuhwhy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3viezbobr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mudyfcqd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ffzromrf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3kappfolb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zlknsljd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cxyjixxg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3yobnqggv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xkgzsmeg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3yqgfigyw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wrpjozwf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3vwegrgbf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tqxfvubc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wgxfyent.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ufwaaqwv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3yoaoqqyi.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rsycdqyx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3nfqnjizc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ymywziog.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rdocyezf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3lkgzsnxe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3icorytfm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3mgklbaru.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3cqecazca.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3aafmorlm.html


<!-- 参考信息 -->