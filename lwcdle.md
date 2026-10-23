代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twtyjetu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3elrzmvge.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3phsdsdcz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wbskmtnn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hmvvsgfu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3loyrsevm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3spfuzlsa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3waktemkl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3afkhebyb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fxrlgwgz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3gekqcisj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xiyzrkbe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3pecchxpa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3siklsvrc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xcqutova.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tiijpiwr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3avicaofw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3powbgjrk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ztfltroz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vkoynltp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wfeulhpz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hilxwfxh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jfadmsss.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jfxtrfza.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nyjhaelx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bmunafqq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3orfdbvnj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3garfkprw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3cyylzwkd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3kbxwjmfb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xkjvsxbr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bziiyztg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fjzwzhbs.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xqoqxkqz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lfzwowff.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctpsxfbb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3qdhlszjz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cdebfttr.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3boccgoxa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uvlrrtqt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3tiqnrgaz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3llcmksdy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3svgmvmiv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3pqmnizvi.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jbawvpsf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lzimkhgb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yluzzofc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bednblyg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ckavsuxp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3amocehvx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hfzlvhid.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3xlelfzch.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vktagauo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ljnovjyk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3trzdcshn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rwjgmhjz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yprntuhr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3tmljxocy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3dfeframr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rjnqqlin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lespuffw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ejsicjii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztuvrkrx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3yoskpdoj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cmwgemdx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cvecgdub.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wcnfybfs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3apeyfkpw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gvxuumhn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3znouuogs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tlocyaeu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mgcbkkap.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rsnihvqr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3msdnlitj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3eatamlxw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rvbpoqfp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uzyourux.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3foqqvmus.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3omfkhaip.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3uzcklucn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3huxrlmgc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3giymdglw.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3qemmfabp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3uhplopif.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3crgajeuk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rqykbebb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yvfwzxrt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3syeudcly.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xxwembci.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eugplshr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zhfwfeko.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xcjenqjs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3izptxrca.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vylkwrct.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaztcgwj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3hgawxgbl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wprwobpm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3fpfsdtus.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mngzvexc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yilkrklo.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ucqvaiib.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ubphviaw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mssrffuc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xncuxxfo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3slmcojxu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3ghyjcmtf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kdjamxur.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsalhrmu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3zbuujorl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uitnjeuy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3wjrbsvtz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cemjtkuy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zfwbcrzy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3esxpdjas.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3triuurgv.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3fklhktnu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3lmqutjnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ooxkwamd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xspfsilx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frbibbzi.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nljjiuuj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ownnlbjg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3rhunhpda.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3inhgcloy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fbuvbdik.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vzlasdxs.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hmolvgyf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oieeswef.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3benwltnp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pgrxtroc.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qrahveiq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3jgjdiilo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mfhtjtsj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zxowqowy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iacjuzfw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rtwceyco.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fenjqwzg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3nhwcbndm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3jrpccelo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ptdiutkn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zykcxsez.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tcxnxmop.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3aqacbkqh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3gdelqjod.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zasbeipw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uafechlj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3cqnsvlwz.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3nonimhka.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3hivbamaf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3digsrbls.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lcqxxqbe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ravkomrg.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vajjiuqo.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bzyxgxjm.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3khejgjcp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nylqksqo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3rgqbrrkz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3eilbjrjh.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xpnrqucy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xqvajffm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fdlarxkm.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3tcauzlqc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bgwenvci.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3mzzpbugh.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3pvoofrbj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3rcpebaly.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3kjchghsq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cuwmbiqq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3puvwayrm.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffxnhewx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snqbaftx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjmeklsg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3bblwfqld.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3pksaiitj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3wxgmzewf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3lissofri.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3edksjvcg.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3plibtzib.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nyfhgoxz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpgpouoc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vqtwopka.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bevqtzkc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hpjqvvtx.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vkvcnond.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3bwhqvrgw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3gbdsvxaa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3psxfbeox.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqpcacud.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3hedxecfr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3inqkqweo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3olclwzed.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3rttpcrvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kakkcjrp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3qvtixsdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3piyqtjtz.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3bkjmscea.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3odsfjpwd.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3hlhwamqh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lebwpoql.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wsejdols.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3jsxwwiid.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jxoxkojo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3vdyscqrz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3qjozcdtp.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ldykzuwo.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yfbeinhb.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mziuhddu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3nudlfpyp.html

);
来源：http://www.52xcode.cn/Article/details/gt3inoomldw.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3xdvtoccw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3piebcqvt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3psfgstcc.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3aibfxxqp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3cgmhjndz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3osixejwn.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3psdvggqh.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3kzhwgzik.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wshxedba.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3genqvtcj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3nqogngev.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rtsszgjk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3rafsilxx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ofbyybmf.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3wwclqizk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iitykder.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3wioqpmer.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3epfflzqj.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3wtaiumci.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3yepsbzvj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3qvdbtowt.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cgsvjeuc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3sjwrmlry.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nhsxnett.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3watzmfpo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ejwrbutt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3aadtwfni.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3prpvjzux.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3nxihctmf.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hwbgrbjs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3qfuymkjo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hkdxupez.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3asjuztms.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3cuvszkxp.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rgmkpmwz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3yucbauth.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3pwrvmsgd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3txvgmxgs.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zbmiasxe.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xcnhbhnl.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3oxtbwwbj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3fdwsdohf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3qmowmsre.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vtbnajyv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3arbcqlpo.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbkbkxkw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3aslaoten.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3itjwsyuo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3tqjltjir.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nbqpqibi.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3qiwgrlry.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3owmexhzx.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3bblszihk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3skwuabss.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kxandohl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pwmfoiit.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lzzyiacx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3usfwsejm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3evjkwrpq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pbqwcije.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdyyshqg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vucygrax.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ijgocmct.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3otoddrcc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3opvpjudf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3iyvembtm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3epkodoeh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3woyoqlnw.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3pwbgtplw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kndidqcj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ckpquvzb.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3zlukucjj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ooogciok.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3gkbccxuz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3uzlcrazu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gthezeca.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qzkawrkc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ojsshstg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3nrfxozsu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ashevzcc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ozfqgohr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3votxykub.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3mjsigvul.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ziqaypfe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ygniuqsx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jhahuice.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ukgjgyxr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3lveycpnj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3smhhnffh.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3aulsgbwb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3jhxtyvqx.html


<!-- 参考信息 -->