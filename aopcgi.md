代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvwpndfx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kmrfmkbc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yjqdzabm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hlwzpscz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wsvmkwoj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kvamifdb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rsnjukgd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ubjpylpj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ihexpvjs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qqrystfc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kmtjbdug.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2buifpymh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ctmgaopq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zwbmubgs.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cxcxfwmg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fjoqnrmz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2lpfdcuul.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tkitfvcp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xoxhwtym.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fxuooqbp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zpulyfgj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2urvjdkbh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lerbycsb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mdgyjzpp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2leayykfr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dmwltdst.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2aupxxkfl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dbfamerm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2opggkhgb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uqwukhuh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2johkgybr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sufingei.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uzcyrcux.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gyejngra.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jepsyzdh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jxwnejqp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2itwgosbh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lrheaxtk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2yyjgsoeu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fdtoetop.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ymsjeddm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ctmncddq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwvdexli.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xekpyfgk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2knxylolh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijpepycv.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ivmgipbz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kixdrycx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nhmhynbo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hymjqjmq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zrskmhtd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xwwcbmyt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cjkafzpa.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rsrjwbrc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkbodrxx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zgpfpehk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2oopwnber.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2eqrhxqto.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2aevuwgcu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ykrukath.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zbzijvfp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2echuuyji.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ojmoofmv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pzfqxidn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uiqmxvqt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2pgckdqdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgmyfcgy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2delmsocg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lkqhjdxy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2vbajbnjd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bhcsxiqz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kyjenwuh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2maedwhda.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xrlienzx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mlgjnfgu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wotgwwrk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wtmlbzco.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2rydqhvol.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2jsnfzgjl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ypbtvyeb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2oosyjoja.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iwnkured.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gyxodkgb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2kafllsdo.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wnmjnyrq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bvwpgipm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2uyqqzonb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ozbpzlgn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yplhzgtw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ayrlzkpz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2caqloxzh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gvrmqvdo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qzsiwreg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fiwxllhn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2bolbirkg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2lqipyadd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2muyzttom.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykijgsge.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tanxdcjk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2nskwrhyu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2alwiesgn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wfmlpdia.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ewqjmcja.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2uymyvyku.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qlzoskdk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2euvqrfvx.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qxqhrhgx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xpqqspvv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ikyemxjf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ynedzfog.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2olpntoah.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2bqlkuixq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bsxdpyjh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2nimdmnwq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2xnutayvt.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vxodkidm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tkktkdck.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2oenkzgdp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2lztcxsxj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pgqdyqgk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wstldnpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfvzgibd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bbkvrcwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqakrkdc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xzsekcbm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2qbzgjvkl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ohmpbfgf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2vigbdmrd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wrksdnbd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tysjqapx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nzipfhaj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xsveccgb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xlzeofrg.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2umlwhyhk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ttgbpceg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vqtgbijj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2yxrpgyqa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ibdoyprb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfmzhzm.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2yhmjofgg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2daxdouys.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ktjdnioe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqolikqp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2lipdyvae.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vtwsdblu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hvgilboo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hummyvch.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2naawxkgh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2qmxmlbtb.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2fljpntuh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2zjgihjui.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2edjnqfrd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2nfuziact.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2udrnyizr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qiwjdakq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2cgsfbkug.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lewuofgx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwwcqpn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wtyfapda.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2etzwijcx.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ggkwijnw.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nnoohwch.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2uholdumy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2zonzfndd.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bxidexyo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2vrayjcqx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2omggrkfy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jjbvueym.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2cmxvjatl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2sbyvclcs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ilbxeypp.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ejhwbysu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2zmuuoaff.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ajmdxibx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ndnkkbph.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zviaevzt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2nhdvxrse.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmexumsf.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2libvaohg.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2tcnixfft.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2cpczbrpe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bhmizstt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qkbosigb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zuyrekvy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ddklrmxe.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2amepvelm.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jdbooutc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2njkpnuqw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kvjqbayd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2jqgcofqe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2tsgfhmov.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbfrtfjp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2mcftumqi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2numgyrgf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2uvxkotxr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2eddhjjxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwbekjrf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2ojzwanfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inbsncbw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rywhhtvs.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xvpfkguc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uhpxkdmr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2yzzowwac.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2eoumljtn.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2kzhipbhd.html

);
来源：http://www.52xcode.cn/Article/details/gt2uihkqchy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2gqhwvhrc.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vkumhicn.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2viuhizaz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lroqhlmm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2yypiszlv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2leffbbil.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2goeltbnc.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2cqynsmdq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2blezillu.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2azkebjpq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tuagxbds.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2drevbgnq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2krpowdgd.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2gxkseyrb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2miflfxyn.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2mxxhtodu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xndnhwhr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2ocucehon.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2qrmzoabb.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2togwgrmf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2skekvdir.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ijspyzan.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2cssyroer.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2rtiglyva.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vxhjrlxq.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qrtvcuzu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zqqjnmci.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2yvudhfgr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2waylneov.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wgudjyhn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2tmexomqc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2knpcqmdj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2etrxbhnb.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2bewdqpic.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iasyqhvx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kxuliruk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twhkxyan.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2volzkiuz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tmjzvzuu.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jufwycmv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2nnydnlfb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xdykscwq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2xsrjrxem.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ahgrxtrd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bvfyckpb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2lfuabdvm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bcfcfbqd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2octamvqw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2typzregd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2bdocdnqu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xxhmklzd.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zzqjotax.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uieqnerx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2safchjfd.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2nuhuujoj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2myivezze.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xfnyzhrm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2vtboxqci.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fohebutb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qtjbjhey.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zgghvsoi.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2soadjyix.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwodcwjj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2hxcnntsd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nlvwgsly.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2znrhrutq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vqnhxeth.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ccmhrtla.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xwkpdshc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ctizjskf.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2rdnmjtbl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2qnwfqlvt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2krscyowf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2icekwnlz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2beipwvrx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dppkqupn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2bixhrsrk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bmnysmij.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qeeufgym.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aygaovjg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2riqezjuy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rngoykvj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2bjmpianc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ekihyzxo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ehvfjjwq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2xmisnhlk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ikkcizes.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2uahcawht.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2tdnewogx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2mzdgaxyi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cimpqyzz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2umvgyfwm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2crgzviam.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2letqomoz.html


<!-- 参考信息 -->