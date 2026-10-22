代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mfaqzboi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mbotmili.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2latymvwc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2uimncfrs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rgigyfam.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tqpbkcmy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hggnwvmx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vlucusxt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2fciwmlrc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wsjgsytx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2fjjgbzoq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rrtdplbb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lqxlfdfr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qgmsluca.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2turdxfgu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2hgrmrxpw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ankjrinj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ybzvzrar.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ksypmkmm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2timqovey.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gwokjpef.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2naohpkos.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ostfllij.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2reyzghwz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fwbbwarh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2bsyzlvwn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kgqqsfdv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qkhwadym.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qmlrkggj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nbjncxii.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fwmvwrug.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kfzwlpaa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wufvwtfn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kirwcnoc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ejfncecf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfewlacj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rqzuskyq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kgvdiald.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2axwlbqis.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2loaxnrkr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qehcocuk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fbcalgcz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fnoziaih.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zyomejen.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctyeyhqm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xrvnpouy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2hutoktms.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jesvwmbr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vippuaaw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ljmnpvxn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rzslzbjw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2shwdryfs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2njcvhwow.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zoluqkhk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xcvvajfz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ttztvize.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pdmkhowv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2laokddhm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2etzdowda.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jteojynu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmsxpbjn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2sstkuobx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwqvfbfr.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ykirlkse.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2kewfoywy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jtrpgvhs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tqiljuge.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nwclzpig.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qsybwcly.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xzivdzcq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2tixrossw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zpnjckts.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2tsxmkzrr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2arlcktxx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2wtkdojac.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2phhdmbxa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sazrgvsy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tfpwnopa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nbzfdmfc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mjmzhwyp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wfcdjntm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2eugmwuuz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ssihqanu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2bvjhjiap.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2krhwjwcw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pzrfounx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxbbtbnp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2clocoryu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xrzotwah.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2eezikuia.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2czusezod.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2uirkiteq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ajzqatrj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ptpgzvnj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhedbgwl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2mhourdtq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2rxiathca.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ifbskpbx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdvktvy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dpeflpjq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2elyxjclj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fningwxl.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hipyahzw.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ftnfzsjy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2logajnxo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2etjgfapk.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ideuvyct.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2shxtfavh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bpmlcoka.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2adkvyajs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jdxnldnz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ffkfhufx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dsbgnnwp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2yjzdhdqh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jueuyjov.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2biyzsowq.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yoagxcmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umtekgcd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2glioeafr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejniloeo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vwswqovs.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ruoibhkb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2yirciqbu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ikwgtzcb.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uddllyce.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kpztwwae.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2axyewvzx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pktfhnhu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2sdkthfed.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2nfsiootk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pvnnhrql.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfiloitl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vajhdqba.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2knagkncg.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mwdessbf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2hfbkeqfu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2knbwrhoj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ieewukav.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dpcfrfwe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2kbnlwnzm.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2nrqkasfz.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fsodnlfh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mnizwqqf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nvmwutwf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lrkzubnk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jwzojyfe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dwimcibn.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2urknimzd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2zfnzjrot.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2scphxvon.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2mfetpdgp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2pqanodeh.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wrpfoqtz.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ceuznreu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2yidismgx.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mazljlnh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2fflbrelu.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2eigmztcs.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2snpiddsh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ezevtnhc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2lhlsucaa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ooyybvgb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvqqeed.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ivcmeghu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2skyahlas.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2mrzhbspr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2rupnvnqq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcbtwrlm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2okbtrafr.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujbwpghe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vxxafukf.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyykjxjv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2afaqkvbo.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndqflbam.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2pheolpxh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2hfmwmfza.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2obhxrpsk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hcxtyxee.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dajrudgf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyayvsoe.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2yzdejhle.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2mcsgrdsu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xmgaddoc.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2sgxywiaz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qrizcqsw.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2byamvegq.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zoycuudh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2liuwffbz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2zztgivsy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2ywpccxgr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2erkzyulf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2hzogmlth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfsaznls.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2cfusixdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyrfilvv.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2viqyqhpl.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bhrmbkad.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ohpqpboh.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dspvksbt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2boxlwwuw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2begucyeh.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2rftncrrm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2ekxlniop.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2ruzmrnsq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jhyueuhv.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2xbcsykce.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2pspplzsx.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pkidxdoz.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2eywaclfj.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xryggarg.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2wmstujva.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2kkyridtf.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2xrolxmdh.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fvxyeedo.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2iocppjan.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2otynsupz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2gnbwssxv.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2cbknqril.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2yoehgfkl.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2fmqujedn.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2lnfavwae.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2tbnqewto.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2bpgkesbs.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2bvhfgzuc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vjliovld.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2hgskkjkz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vbkmxcxk.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2odwjjxen.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2grdjtygf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2movruhie.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hvxtufnb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vpbxrnoy.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2ryyljmlg.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2mbrjczto.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2bhwhbndr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2hnoyonbf.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gjxrnvrv.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2onasijkd.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2clblhmpi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2melsheah.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aonexgwp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2karakoml.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hfyjhzot.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ystrwogp.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2qdqakpys.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2gzqsjmqi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ezpbzwhg.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2qfjpltan.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yewdjxqt.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2dnhtohqv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ythtttas.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nbiwlpqk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fujxqqlf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2rcwsmlgh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmdnqfil.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wtpkvsko.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2oqnaxuhi.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2aztkvbmp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pdhbpgdb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zwynejrg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iodyjlnz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vxntbbjw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ysqlecle.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sefvutqz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uobwztaa.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2glkyvsrv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tbildtdo.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2rdfewjpa.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2xevngksx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvvcfvym.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pfsppphs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2zmeoadls.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2owxwcbvb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xgnwsgao.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2lwwwqpjj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2fzdeiixo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nvdrqbch.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2wbvcplzw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tiyfsqmx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lgfvfemt.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2mgmbhwps.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mbeqbihj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2shhnokfj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ybadubjl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mhxrhmot.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vhncsvpy.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nfshzupe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tvjoxsur.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2nzdgblkq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ghkwlghz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wushuhhp.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2cbmwuzhy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2muotqhgo.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qegvfzcn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qlbrvquy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2saizbkxm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2cjyagasr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2xvspikkk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2drqimdne.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vpdsdnsx.html


<!-- 参考信息 -->