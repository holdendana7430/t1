代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2asiipagu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yxtmszgh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kmqnibma.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ohwgqjpb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qochfqwe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oivybyqu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dfobkqmy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2lbcolbjv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2elffyhky.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2dzcpcfdz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pgsjvjpv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fgmnhoxr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vkgmwufs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2sawwjyay.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fqfkxake.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2fzdrkrup.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zotupkke.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2cfcelxyg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qgyicuhf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qovkruxs.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ehdvftwh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2aafwynms.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yqnzvska.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ypxivbix.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wrrsxvsf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cjmfndne.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kshlicds.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eqqhcebz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2thpxjcld.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gskakrni.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nezwlyzq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2olxibtms.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2wtmtuhay.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2hvrzvomk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2czqtvnit.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lnwhcxlg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xkwaelhh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pbdsunpm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2szknahxm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ojwpexlh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2jnuacyll.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2iwweninq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2etmjsxzg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2uivtrshz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cexsubde.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qdvjlcbr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2drerjslt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cawzpcty.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nnsnvvsf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2wrhqmvmv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bjaugpve.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bxpfnieh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zkllybhg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vygxucjs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vrlmqokm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2eqlupejd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iinhpjak.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2iinomjgq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pmyqutyw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2neiudaej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzkjnqul.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2uzavnidc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exkcbzkc.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ylnhuycn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fptxfvbx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ydrrvqzt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2kyypdrua.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fodiavdz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cylwwlaf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2hgxeumny.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2soizrykm.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2yshiykee.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nlqhrbog.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2izfnfodf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kgupsgjg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zvmcwxsx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2csfktepi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2mpytyqop.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bgqqdupy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rckkzwgx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2pxikcrsl.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2anmqdrja.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2njefsumx.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2rwsuwwvy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ufejqhnb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sdsddufd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2opbvqjcv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tuxubufi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2uaczhzeu.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2umfsxyse.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hgmzdpbx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hxtyprgd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dxlcesmd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2tliwouau.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ncatltjt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hevkavqu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lelmltqi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fwbxftcg.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2qpphyihg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2juqjlsys.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2gtgwvbgp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vovhcbpt.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wurymsvq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zxijxfwd.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ynvwacde.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ittzjapp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2oxtoydij.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2uagptvyp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2rwtjbkhh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2qpsjpglf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rsmrgjjn.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ajsrdcjo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2allyftcs.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2qjrrqlof.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2sxedmrvq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lpkxrknv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2wfranfdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhlqbxsz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2exzcrgyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsndffem.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2avjxqswp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2axriibkw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bjyyatqb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mewwkmjl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2axwgihqz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oetgwbub.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2idbhohoj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qfwnattm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ldpmpifm.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pivjsziv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2srmxagkx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hlqquhvj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jskicpwa.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ytgoiemj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wrcibarg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2basrcqny.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qyisywph.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2fcjkkuds.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2hxmimirx.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ddmixcri.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qytggdjg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pumwhiwy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dqsbrtak.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2colazlpf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lufkpgbg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2vvntkdtr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2pofiwsvl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2drnhjzvv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cfvbvlvo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ffdjgerq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xzsmafoq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2tawnuaaf.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bojqwwag.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2fmsomtrp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2cmjhoevq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kjlsbtxd.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2ygbhgsuq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2kdjmabzq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2rnafmeso.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ngxoaiqy.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2akzrhgix.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2gozaabto.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wgmvwwgs.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2zjopoupf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gxixgwxb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2beuvxdyh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vugdkxmc.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgaddhax.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2gfyxwuuh.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2iwtkuqtg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iiwyghjg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2iezsufuf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ydjjqwzx.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgqxefff.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2cuhjfinn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2pbqsaibf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2mclixkwf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lxprnilu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2eurcbxjd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfdzqnsw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2obwgtkmd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2wckwkhjz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2bqrnsjta.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2rnnstndc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2vhgtfxwv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2ciylgusk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2ualyqtmg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rawjprxt.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tpiwvxbg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2qjhivthl.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2akyxqbug.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mvrqkasm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofmphkri.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2ustihapb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkoayumj.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2peoniluh.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bbtwalwc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2yxsxpdsn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2gazehbmt.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2tbkqabrz.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ccuswvcn.html

);
来源：http://www.52xcode.cn/Article/details/gt2dhyavcvz.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2mvzmysnj.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cjzfcjrw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cchxnorm.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2jxyzzpcn.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2xaaxslte.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2tznkqihz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zqxqfyhl.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2uodrrxet.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2imbtcqpc.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2sssovzxi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2wbypetui.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2gytgvhap.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ksaypaec.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2cauaepie.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2dssfzdkd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2quknuxbj.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tsfbhkhc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2omvdrdky.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2oaombdqp.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ubjdbfuc.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ggkhfymy.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2iwqhdmef.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2gnhyngdj.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2esheqqyd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2xeifmtku.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2jkknhvba.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2vzqcbtfi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2yedatdnz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2sfyhmuxg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2auhavaem.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2lrwgwrzg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2fekgccbc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2wezatfcd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2gmixnrbz.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qhckoekp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2bwobigxd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvyemafn.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qssravbk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ovbnqdhp.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gsxcsxha.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2hxqqrlus.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2orepnual.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2pnxkeqxg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2gsmfjyap.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fvjcoqav.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2grldkpoi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2nvtnqnbg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2grfyecne.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2axvndbmg.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2efvqhesl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2srcengrt.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2zfxnjysn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lecezulz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2gdxdczij.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2sjoaexow.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2zwjuodid.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kanyzjae.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ynpkdkbn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xtwvungi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uxvpesdd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lfyafvjd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mdsneebs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjqvysvb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2oklaohbo.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rugcnpjq.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2xtufxclh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mzwwiucq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xvgfpxjf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lqgyhsrq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2drhxdcgy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2mmckbrcn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2efvowafa.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mkwswvfj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2nsamjudn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fgvaerdg.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2hfcushxz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2tijiaibi.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zkdhkjyl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qxwseizl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ybxcvxuc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yzpbdigf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2unsagjwr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2gpsideig.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qdedbrwj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2pwduiori.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wdutuqmz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fusmukuu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bolqilmr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2pmcinqot.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2aosiyoua.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ixxafgej.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2gegygrvp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2lzegtgss.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fhfekueo.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2rcthvybv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pjzoacym.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2usgllrcr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ecpmsnqz.html


<!-- 参考信息 -->