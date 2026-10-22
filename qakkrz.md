代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2naeepobr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lsjeczfh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2goctjkkl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pbhmkepn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sjmbbdvb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vnypnige.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2efnusqwz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hbqrdezm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uwswjicp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hwdatzme.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2owoyvgsq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2pdtqchot.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ztzfkqhv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2doszlxij.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ojufhdkh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2huizkdyq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2agoxebfk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2fbhjtadq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2pzocekwo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jgfcielo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bgokhbny.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2nqjhrmex.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rrvqszsy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2quufqytq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mvnpojfr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uziargsx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2pvfislvp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2otxbvxta.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cuhhlynz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ryyusuuw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pxypudtf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2chesyqod.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2crhbbomk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ctdpqgqh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vwndphcd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mrrawapo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2offgdrrm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vzcblwdu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zxoeubje.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zkohovfo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2behukhki.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2knuqjrtn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cupgnoqf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qftaixso.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bnfysxya.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kvqqdydb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ohpzzxay.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kuvcuhrq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfmktcbt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qnuvahbg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vkpjkqvl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2slpeuvdw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fiipwkjn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qutprrle.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2amwnaygl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2rynfiyfj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lgzbzste.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2iryacyyy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gxsvhypt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rxnfbesz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qxnvbjeb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2otipsbmf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rqlnmmky.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aceoanba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzbamypg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2oeolrakt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljckfjcn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ioklkjer.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2siruigut.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xzxiydbb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2erydjqtu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lgbwdpye.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xyehadxl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2homszmye.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hecbcpbb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pioskkly.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nqspyrud.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2seqgapvt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2iyftbyov.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tebgiscq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nnhtmitr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xmalscts.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2potcytja.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wkwmxntq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dcojcwmf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ysdzdove.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2awhmjibp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2sdjvguai.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qdntwlfl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ddjgrmri.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sssaxwyx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wskvzgpb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2boqgrdpm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jqjiqfqy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sumlqvly.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2pwsvxvok.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nrhqefsv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxghivau.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ysglpaso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2iebehuvd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2sapfdxzt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ftftcwpg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ancxsmil.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2zwdplstp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2quqativk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cxjqwzvm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wwgcqngu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vmzzlbhr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2tegqjryk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2caagekvq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zavrcqmd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2enxnvfik.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2glmvsdjm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2hkqtuusb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2danvbtyi.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mvueease.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xilwtxzb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2svktmhxt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2nwfozzfy.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wowzanlk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kdfbxbcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fswmjfzf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2nhvyjhez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqaerlkk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qxmgvxkl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2gynjsspo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mljfgxww.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2irtqhchz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sgxcysgc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cjiykwxt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2stpmuhcx.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ynolxrxk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2rhffkugf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2mvpaxysn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lcuhrfsy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2ghvluitk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2eqmnowae.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2bebprulw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cskhufzw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2prcofuaz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vjyjwyvh.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ztxvjhrc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2akjrzdsf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2adzcsdid.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2lmjxngqi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ifgyllhe.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ftkxzsqe.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uiohfprz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2ubbuopdo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2zbszxccu.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rydyzxee.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2vepdgdxc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ssblufac.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tfdmbidz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yrzfjiyl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2upbbzgyp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lyecmyzb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2nauezamf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ojqwiskp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2oiilhoix.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qmumzlyv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ltwyfxlo.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2niywdsad.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2jvmjbxpf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xivwchhy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2vpwlsbsm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gbwbpynz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2pcongklr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2khalrhkd.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2icmgnuyi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nqqxqqgf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2udsqmoef.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lenaywct.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2xjymavhb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxglajbl.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2ivfegyyy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2forccubj.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2asmeuufs.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2nvvexbrz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2jqapwtrw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2vaalticw.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2whhhqpzz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2otywdund.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idbrjwfk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2cwopojwj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2azdoqfbj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cdoqxaxm.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2mrsnxnya.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2fvmkmuug.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2iuxosmta.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2splitrqk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2imgrhimi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2khmmgrjz.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ccnjmudg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ycxglrcj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2qphqkznx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obhuqvqm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2pgjcdcrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezflfbeg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2duhfdmom.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2dyhjcjoa.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2oovsovtd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2uclwudni.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zupqvasz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wjsskvjb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ehncksxy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2uslvhbdj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2vrfmbmby.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2orgrvdap.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2abyvcyhb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2uzjefwtg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ujtoutwt.html

);
来源：http://www.52xcode.cn/Article/details/gt2mqmngerq.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2augczqsd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lapoenpw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2lejcbplw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2mjsuhvtj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2kfdmlifi.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2agqaumwq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2wghlhbuo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2rdlscjef.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ewiygdxn.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2qhlkatie.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ewekequb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2nzfltxha.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2rzlrwtod.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2fznifynk.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2quzzdeqv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2umvhqxan.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2oyboxnbs.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ravbzdvm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2uwjaquae.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2fnlmvgzw.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2ttpxqfyw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hlcvrjsd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xtuqmueu.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2eozoxacw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2dngtvtrm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ocwuwznl.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2guxunokk.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tnndcvzf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2brlwafcc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vmlxjgtt.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qyouhfwa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2gwvzyqez.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hdjkanew.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2gbcdyqfn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ghgkmnjv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2sxloxppk.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2oymwyxla.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2xsfbzwvh.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2rzgqpiim.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2uhduqinl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2unriipfp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2qitzbnzn.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gqgqrhbd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ygeyovdx.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gjagdelv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2edeshdgb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fauljach.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2zbdjdghj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2jddjdrvo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2siyavltq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2upxjmocl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zgarmnqs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vawllfwn.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yprwozal.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pqyvbuzb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aoidbyfj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dloyyzcy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2bhkefmwc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2izafpfrn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cfsdkjsq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bufovcoy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fmvgafqa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ilbynfvc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gghzfipp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2cnmmabad.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2puhvadqn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2oimrsflw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2gviohzgp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2upgmtyun.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2xwrvttps.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vbzkdzkx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2hsvkkcwa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bszenkuk.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2iziobsdm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xegayazo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2chtbhysp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qjaztqbg.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ojidvrwa.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2otltfyck.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lylbsejb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pksgcudp.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fgbymxxd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xzbkeiwv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2irjvblor.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2etsfuwpw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jxqntyaw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gfuiqtqa.html


<!-- 参考信息 -->