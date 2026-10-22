代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vxegajxq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2okrqxtpn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2khpajbdh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2eunilgzh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gsjoewue.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ntxbfjtq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jclhlhdz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ebchpsgw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rxvckgsi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2elwxwqfz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2qjheliqi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rcpgbwyr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fbrsvday.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2hwklxibc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2utexaxyh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xxdzikxw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbllkadw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dmrtlyms.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hfpnqmkc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovdzndcn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nyyypsiy.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cgxewuwt.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2orzqxrhz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jzmzghvy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jrcqlqew.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jumocidg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iogeggqi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gxifyloe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gtnhsufl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sobpobac.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pqntyxov.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dhddbyge.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2yklhxtnj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2bwrzingz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gvbiiblw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2avsmvclk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zvlfflei.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fscmzchb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2neglylqa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2phvxzvau.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2peawnqkp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xscktekm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ahqchhfx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2cdhxvpqn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wqmstsuf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ylfugrbf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xiabucti.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2iergjhxf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2folsjzmq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cqbzcoxb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wqsmtqbe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2oczclatv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2mmrurgom.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2slvrgrqr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sbhshgne.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qqaqykne.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vzobzzfp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2febplxog.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vsgbedvx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cvcomqec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yotgphbl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cbrsiaax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jefcsqoa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2heiwtwtn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2oaisuwld.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pbdczuor.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2itqpltux.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xjtitfwf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2oesyptzk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2sprvnfzi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2woaqbfug.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2hogbvrhv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tiojmytu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mfzlcxrj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2feznmbdc.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dxcicxin.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jxebuglp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qzibxhxk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2kmrasfvx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xzbsvscb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fyilzlrv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mqnbdsnq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2redzzlpd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2cyxndlfk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2grigdbvd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lcvmmwjz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbmvtsrs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2jiohisvh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cwbdfrkk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoutfmbc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2uszcasiu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vwgwtfyu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2loncbxyl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2oossydrx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmbrpfwh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2iufnnxvv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2syxcwhsr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qmjnuchk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ktncqghy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2irktmlxs.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2olldryey.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kgcvzowf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hyxathbz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gcnqoudl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zrxsdgvy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2atlnioeu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2axnytild.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2llrcjxot.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2atxnkzip.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cnnsuwro.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2cfgdjztg.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nyqpnzez.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wjxfosan.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2jwskryef.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2sydlahqt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2atycwaps.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2obpocqoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iuqerayx.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vzeqdpfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqebaqcb.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zsxusxhi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ysfxdvda.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2twkbqoih.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2aycorbjj.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jptkpvru.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2smvhdrzp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2sudzsldf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2clgmovkg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2joygverc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mktlyiiv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wlsgwllu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2datiycbt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vbhiykzo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2icwnfyuy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xxyrqtot.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2igtaspcb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmzsula.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ptwujrbv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2daylgohn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2efuyhake.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2abkpdudk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qpozyosf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hlfwtwuj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2vgvilzjf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wzkwbmhf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2waifcvlh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2nppajkaj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hqdyxqvr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2uohgkynt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tdlomxeh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rnkhnhgn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ccccjvfb.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rqmgvxip.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wqdcqfjy.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2mojcrzfh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hpjblbug.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2lmcfphxt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2taytmrnv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2osiprncq.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2vyqetjgr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2htsqpysg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2obmagddz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pkuueiqg.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dhnicvmz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2jtkuxxkt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2uolzqmhs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ueduugnf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rjzuskmp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2cauytcls.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2czjuviiv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amgptlec.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2vlpxxxwp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2pugjcvhl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2cwhxxbbk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2xfdhabou.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qezurofb.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2urlgkzjj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2iktspxrx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yinkzmpf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2yonzgymo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2szqmbhix.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2azxqneib.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2hbilxatm.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2bjpqrocq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2xolvcgyh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2adkppkee.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2gdtjvxfn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qavqfmhn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2meyouwgj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2eqaspptv.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2ebbjxyav.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2onzcjmwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhiefujw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gfyebqrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxxjgsjy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2arjnynie.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wjgkpgep.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2vquoghjn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2wxepticn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2poyygarr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2vrglggyk.html

);
来源：http://www.52xcode.cn/Article/details/gt2xbinvyyy.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2wuseheto.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ixmcgggm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2bnivbrrp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2byxkzvnc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qiwsfowv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2ndnmzpxr.html

);
来源：http://www.52xcode.cn/Article/details/gt2fekwlqbc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2bfyyeuvv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2yxfwdjsp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2tsqhmogn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2hccvomye.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zhgrlvae.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2pqfcmkrj.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2igsoaibf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2nsrirqfc.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2ywmtkcwy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2udtblllv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2jyvuyjob.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2jawvltlk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2jhsdtflq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2erykipuy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2czhnpfkp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dcuzttvk.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2gujcltpp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2dxyyrgop.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2owqsutvw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2xlnpkcyp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2wbeslzxz.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2fdmqxswn.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rrmemsex.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2vxevkxcb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2blzpiaos.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bwkiwejn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2tghkzcky.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bpuuuxwl.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zwskpmjj.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hwykivyi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2oheujtbi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2svawtsjz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2lrzpojgm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2wjwrjicj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2bqsltlid.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2tuisrwfr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fgovsybu.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ygyepktz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2vmihnhbg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kefzsobe.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2sjwmrjqq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2nuejtund.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2mhimxybp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2gellwaum.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2vqtlthhs.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qswoxjnh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2covxyvll.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vyvbobtc.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lrgknwig.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jwjaomxh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ruyhlmrx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzqprykz.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rnrucfrw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wxnepkrs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zajudezx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bwhshtvr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2swbyxwgv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zkjrvfuk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2satcuofl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tciozlzg.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mwrkhyfn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vmabfdxn.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qxldteva.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jpncenpn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2vwptizzs.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2easnuwpm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2tyvknuig.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2rxoyjfzo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gnwhqdrz.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2bihahhyk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wsvsexow.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2zxcxbkqp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ptyfvahv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2gsonmiii.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xojsgljz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2comddghm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kwvtkajf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xcytscii.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jvhkdpik.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wwbrocef.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ictnedlc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2bwfqhblp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2oskwkzgb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2odeifiuc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2dlwwamim.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2unjnfhwo.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2zsrrbhfd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2fgtrbdaj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2nkiuokpj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ehrnncqk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2snbouctw.html


<!-- 参考信息 -->