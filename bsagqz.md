代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyoexqwh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ojvzcvxo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2obhggqrp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zacacnfk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2opplvwwa.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wwnnwbgw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2pcpciaop.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2sbqhgarb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kfcmfqrs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uxcpeeqv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2dccyodbs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uahtwbnk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mclnvyrt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dzscqmjw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ooorwspz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ruzxtydc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qdlxrlqm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2cvnymshh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2stgwajod.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2isdbnifi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2vnragcwx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ynajvjoz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rqpjxmxz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yxeevavz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eecyfplj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cpuefnnl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uwolitul.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ixzzknlg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nfcmeruf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uqtjbzwt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wqhxznur.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wrstprbu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2oktfhipi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kkpjvhim.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dgltbapm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2scgycvjk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nvsrojcr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tibbmvgu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2mwcwqyxk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2rppzspcu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zedzjdds.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ztrrejft.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2phxrdggp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gvacjzas.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dqhxkpgf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ifzxrdll.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ajlvohhu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2rdxppfgo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pftniabp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ojejflqi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2aryhdbth.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pzywdecf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nongdzzl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2jgtejnwb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2htnvqpkc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nbfjbmzg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2akkvpkvt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xfnpcjzo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fauoizox.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jdhsrluj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hxldgyio.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pinqyujs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2whgbsyoz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bjhijvza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyafxlxo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qhkybltg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzqxsycc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ieuoesei.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fataoxbg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ygnbtxvh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ldzxwmwr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cyhywceh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2sjketylm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fpthibox.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ijpwduaz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2sywljmbh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2woxfnaby.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cgoobkol.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2uvvssegz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wvlxnqyv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sapfphrq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kceagteg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2loolklbk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2gfzjfhmt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2lmejpbpb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vkmumouf.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rpozeknb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jtoqyiyv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qcxyhaih.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ciqhksdz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mgeahdvc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2otswffat.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2trwnoxwb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cuemeucv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kpnstxxx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ljlkmnyu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2agdndtcn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkdribtg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fydujhus.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2wvobalqk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rfotkhjx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ppbvlrjq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ekfloyzu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fbumodbf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2fiweykyh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2imcbfbob.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2yeaoftjw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2azcqkjry.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mtxitudv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wyffofde.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2duxytkwd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xekpqxhf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2awdjxuxt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2cglqeols.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2uotqihzv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2iqmamheu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gyseaiqv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2smujpeum.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2qldddlvj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2uqfvykjk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wkoenfuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aflakiuq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2jqdyrkis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebfwqhad.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mlcybrcy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2tmqhcnuy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lxxdigxf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sxboioro.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kpusrans.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qdvnopab.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xngewrdt.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hpbpwjzj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xlkjxiew.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2szbwtmie.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kxoukixl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2inwuwext.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lvqjfota.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ggakryef.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzjcfwj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2odeshvfg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcrdabl.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2slvzhyhe.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2skhfpxhn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2pgyyhrxl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2iyhwdsxf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yuqzkkfj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qtqemzod.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lnhipzgy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2qiurilbo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2kygjryzq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2helazzgh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2qlrvyqxo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2jizdfqzb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gvwrjzen.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wyqisiqx.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2crutjcvg.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rwzsousm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vshvypgv.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2zjatyoin.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qhevwnyk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xximskau.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2ibhvdaga.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2soaigslw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ieswgioj.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mimdtzhz.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2mwcvgbvc.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xqtayiro.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dmuapnoo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hxixclts.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2jwxzcbju.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ihwqwxeb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ucgfptlc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2jhpdjnfh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieszmvcn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ibzqsxcz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2orlgqeeo.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfxvatn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jggqlsff.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2aazubwyl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2zvoyrmhb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2htvxpeyo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ekyamdhu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iqhkuuru.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctllbmtf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2zvrehcjk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ubtvvltc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2guxqxhhh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2tkaxztrc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2tcirborv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gojnjzuk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tfvutdix.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpprbidz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zevjuxjg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2dlqcjswa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2uwmsqate.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2vfvvshpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dffkngec.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pppxubzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuwzlxtf.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2ycelfsdk.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2tpoiwmfz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2lecygzvk.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2twbfueyy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2xgiboclw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jgnnzpzr.html

);
来源：http://www.52xcode.cn/Article/details/gt2czbhfudr.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mwwxlsny.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gtujjoet.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2mrctljjr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2ofuhwnkg.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wqdmqisf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pccawtgt.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qfkqsgpc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2ywlwynbx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2txcpbllf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iviljxxz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2tmbqypva.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fychmxsu.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mquufkat.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qrpkipbf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2etdbtcrm.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2wsadmkfj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sezxhjtr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2phzheovg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2cnsljjii.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2gmgpxkne.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fdezjqjl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ufyzdvmo.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mvgzhrtm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2zszniwau.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2fgwygisy.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2ovbeepew.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2lvuhojhr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rzliofgz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2ydckxkrs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cvcandyw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2bniarfum.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2cpspbtak.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2bukhhznw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2sdgdymzh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cywgghym.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dpenngeu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpeizjzt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2vkxoskwm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rsojctbl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lfargaaj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ftusyhtz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2sumlvndc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2wahzatge.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2pqpnfigg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mtcyesiq.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ybsdirjs.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zoslhvrj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2bredsoqg.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2dotyfnjd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2xbfprozl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2oojbynje.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2clhbvpgd.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2avsaggqz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jrnondid.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ikgilkqy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2horsmkty.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lddyohev.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zmjylwyt.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cjnutybq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2njxsxnjk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xmibvovx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2swwhjwul.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rkesndkh.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ypavxvgb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ygcuggqg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hsofqlcb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dyhddcwr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iprfpdmr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2haxckwsv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2fbukqdzq.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2htiucdst.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ylenifol.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2egwrxvoz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2bfmwmhpp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ruxqwotp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2mgsmuzhc.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2nheltnyz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2huppkens.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2lsskqktj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ndztvate.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jnnylsdy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xhsjenkc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2bkhggpqe.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dtoqfnpg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2klqqxsvu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2cwjnholg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2sxpiqkgf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2gpixlnlt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wtyfljgu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xiptimrz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2yiprqquh.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xrsstgyf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bqqzdhnh.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2nnxicruq.html


<!-- 参考信息 -->