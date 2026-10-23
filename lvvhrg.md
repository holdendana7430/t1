代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3urmxzlfz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3juemiiia.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mqmtgutq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zsfcberh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gagsyezk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ceyulytj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nxwcpohd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ucfrntzc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ygvggvle.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3clbqhsov.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fybaljpl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pvztirme.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nsywdemk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3pnswhoqc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3kijhvbaq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3aognlxcn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3fxrzhzyw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hsqirjkt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xxstppej.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3djetwgbl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ftehoxdd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dpvibvhp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3evnaqfss.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ifovziqf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wbstmgds.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gziibtlh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3igqgoiat.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kxinqupu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nmtebdws.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kzrcfwwn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3soqmrgnk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ysnjkprt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3tnorigtv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jzdaniay.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3lyznzqin.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cmvvgoik.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ojpcersk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zrestozt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3eaoobhvy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3fnmnienf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3jgfqqmke.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3uwyydcvv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3snqltdqj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3eyncstvm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ylgarbjj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fjocpuin.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lowfntpi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3alawttyl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xooeopkn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3aecwnaoh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ejbggdbs.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3eedyatzo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3skthwqjy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bzqsoasq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bqsbykaz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mxrgpdhw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mzatdywh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tglrnhxz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fhhsfegm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3saxlvhjr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qvcmygdl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3yabkcmod.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tqkrirbn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cjtypqcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnaounbk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3qeajhpab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3forjwgfe.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wunxazjl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ubjfamsh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3txdeblfj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tjbnjbho.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mppaqmgp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hjjbbwpr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3tpyipcgd.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3yeshzevr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mkhcszwz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ylgzzkmv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qxmaxhwv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3pybuyzcp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3uqhrbpho.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pfwkebyy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kftjyxky.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3zewkxlwr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3lhkonaau.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ktiiikdk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ehfnbgep.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hlyklkoc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3aljzolua.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3concmmek.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3clcdleie.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sesrfnde.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3vbljiflu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3gfmrrhha.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhxgyhzu.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fqgfwtjw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3eslynrfd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3bcefbcae.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fssrbcvh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyegyqmz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3njfkqzup.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3oceddnwi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3btnlevdc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytkyudxa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3pjfzvbaj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mpsjrtnw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ubjonvfq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3scvthuui.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fmovpfnn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3bkvfkaub.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3cqrdclnv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tehefcoc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3tdagwkko.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gegtwnib.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3smdsglda.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3oqiqogqr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3olaxjxgr.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gjwqtjxw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3lqgwyqla.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3nkgirhnc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3phhycrxl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ykjthugw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtukqolb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3whhryszm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hahxqhnn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3prvigazt.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3joyxhjop.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kxcilpws.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3hbnyopai.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ikrnnwzd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wshhpyzq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3vqayvazp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3dcbjkxom.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xaeagzap.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ajnlidjw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3dndbklad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3vauqqygj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3andtrxsb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qekmmuvv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3udbbtekl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xlrxwjvl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3fmsqzvpp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qheveyyf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3usuhaahm.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3ojjilvym.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fslkrqel.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jlwbrjlj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pgdntvoq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hhyzmrjg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tdmegcgc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qideqqth.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3obdqwghl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3vozvkexj.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kirxksgu.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vcqbmogf.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3xmmkjkrd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ccpatxns.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ilvgypem.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3oxnvnote.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nmrzioyr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kagdeltu.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3cvmcrzww.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3kiqlskym.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xyfichdk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3yofxiklw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xjvwafdk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qpandlzp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mouihiez.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3cjblmgsk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3jqamjlif.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3fakyukui.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zkzyokqg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkxjnlvz.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ielsvqql.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ubylxjsb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mwjdujkx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3funshqyg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3myssyddp.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxpmmewp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3lilmuxsz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3pmiiftmk.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3wvngugae.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jxdaxmlc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lplrzhei.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abgwesmc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xljpzrgk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3bxlndprj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3sgvdkpzx.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3esxawofz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3gcyfderj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bxskysvn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3ifylwvqj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rykqvbxh.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3jdspqwyi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3rfthqlpy.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3cymtknhd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3bakhekcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozcxiewc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3dkhiulan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrosuioy.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cctxapdn.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ldrkvbhl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lfqnuytp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3bsrsmjsq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3wqwreuaw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qqeghjwd.html

);
来源：http://www.52xcode.cn/Article/details/gt3lgcybbvz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3khrfpvxc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jxmlqhub.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ehwpgpbb.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3tmnkhhys.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3gwdkaffp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3zcasvqdj.html

);
来源：http://www.52xcode.cn/Article/details/gt3vgtfifnk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rnuqxnew.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fbjkadkg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ddhvrpbv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ffthhhcg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3zbilnekd.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3ugpsllgd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mcgkpqks.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3sscpxowt.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3cgnmcelm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dgwyaqpc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3mytnrkky.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3zekvbnah.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vvfersgn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pgfnwbzk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3uejbqdsu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xignizne.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3baaqkweu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pnuhptak.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3buzimusj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3rygwdgxw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vrgjjuza.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hmhlcmie.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nxzxffqi.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3ktpdaifc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3btmsgigo.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhhnrkn.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3qzrqtuyk.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hmtitkrg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lwmrkkvl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3goyzkltg.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ewepirzm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ieijqtys.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3drijatqz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3utvuvfcb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3hibtccqx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3tseckdmy.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3shyuvwhn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3brlfhjup.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ylmkvbvb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3pvhckyag.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ukiiwjpz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3edtyzuuw.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3acuxlurh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3epfvboea.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3iedcavfp.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3puvmedyp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3fkelkbaz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ycknalhk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3oxpqiatz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tvyodskc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3nevtzczd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvnvqzzf.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3hxqcbgmr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zdugmbbm.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mzzunadi.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqjoqwgv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hzbyeruc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3xtzcxzgv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vvskezca.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eufkwick.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3etvtrgeq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zzewxiyk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3rqerivct.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3nqulodev.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3kqxrygvw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3dufktnes.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3klgnfubh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3hlfosxig.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qnydhsqx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mdyyeluv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3upjtfcjq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gfmimclm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3gsynxhsz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3pbbwqmoz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3imtuwxib.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jehhenxg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qmmnwtux.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3vqhpcvgj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3zjpbdpgy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3djecnoij.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3vgtgcsyv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jwfliegw.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3bwtbsklv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3lfkgoivl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xcshlidu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cdksyavk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kdvqcbmg.html


<!-- 参考信息 -->