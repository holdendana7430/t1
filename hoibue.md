代发 wailian999

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uoxmxzwt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qiqadqre.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kuaiprbu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2nphnhgxb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2unzkmuae.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mmwachub.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2brxcrgga.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2trtqqput.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tumdcvyn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yswwcjkc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mskdgnam.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ybznkzfa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbprebrj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2eqiuwfox.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zztzcjwa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aqmrtdiz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jzpbzqqi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nrxdoouz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2aedcqxlz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vsqbjadg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fyqoyowo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iqyjwcpj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hdoksvnk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zlvdzhvj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2mwqgnpwk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bgxgblzr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yzctfjim.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fuahxphz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zsdqjgyt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mvnrhall.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qmvtzdkf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jobhsgxq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tecjuqsk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2chdjrefj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeafcqsh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wpqgahua.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2liwexjkp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2biqunreo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zpxkudnh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lrizepvk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2sqxbbsva.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yozbkezg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cwmxkksx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vhlqmwxz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2icchkzzn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2agykbjwa.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pkuxjxlm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2urkstehp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jzkzpmjs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yqttsrba.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2iqhjvwgk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2aebswpfh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bqsgtfry.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2weweusat.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eniywhzr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mpmfkqdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrqkiuqe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hfxqerhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blhcpwex.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ebrnzcyn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vnyzeisz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mglhrzup.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vkutlugb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mpwmnbac.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vclaokef.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2yjtoblvk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2iqcgsqdo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ahhypczt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rzigtcas.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fjmqgedl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2lbpqeysw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zpvjcpfk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dsvtvniw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xibanyel.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2nxccqgwc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2uswitqur.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dqdyikjf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2wogqlugz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xbhvvhvk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2yvyhiqca.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2tuenhtjh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2oguabswh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2wxrnxpza.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2bcgtkbtc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2aibqwyoy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmpyachh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2kwbceans.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wklhmvcz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dxixwqqm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dbuqyvnj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ucjwjthr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2wsihfsxo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2yyfdjtna.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ygmxphac.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbyaxuva.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2sqkwdddx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2jjxfcbol.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2vsfntrrh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2czytaxjq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kqyssbfj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ljqcomdp.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2qlkkycbv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2keevkten.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwwzimzg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nixadkdi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2irrsxgwp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2qnjidvte.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2rhpqpelv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nlrdzpwd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2epigmael.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2lyhogemr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ikyyikyk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xndehlqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bndwixvk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qvavemsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2naxxwqgs.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2dgbgtdsh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nfwcjuia.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2mxggdwpm.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gqcduobc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2tjqzksuy.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2huekvkfb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jqhlgjdj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pamrjyjt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kicdljye.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2awxvehuo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2rzltaqmk.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hhgrhhag.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vpekxdcm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bhlxtgvt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mkwkxpdj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2jdaydzpu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kosamqee.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lqwkbqfl.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2skgygqug.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2gcxogfjl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vnvmcwyj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vmazzkwb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ohqtfpuw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ljfxhbmc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2jcbnvcvo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2epodedvg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xgisoibc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2pbmljraq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cyhrkwae.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2aozbqnzi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lkoqsglv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bfijubqe.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bqpmyelj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2bkyhhbyx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ttayxvct.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2uigyjvlb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2nrixdpim.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2tbmclxtu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2awgyplmd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2syqsvddk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2irmlcuzg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2pbkehbaq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2irfasnvf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kpgnowhp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2pnzpcghj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jcfaszyk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2verdgzhn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2juqjbekc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2dlsxnykq.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkiaarzl.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2psamfswe.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpnwtxvf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2btoqbvul.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcaetaae.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kbkafftc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2kudhvjit.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2gusirupm.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2cknggxhx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mxiaamoi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbmivndn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2pgfpmvyk.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2horgrkar.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2vzsydbyi.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2biavhyef.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2uexnlscs.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2iyxezzib.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2kghfgatz.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vvvgipey.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2eahodcjk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2rhjvvvav.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bobxllhh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2cyarjwqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2darwtbcp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2gbheuvly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vauqaqtr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2mmycmujp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2hlmpdhea.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2lqagxhkt.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wcxbgwpn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2tnozdnic.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2bghmibmo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ratwpekc.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2qjnrtiht.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2muspauav.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nyugmhit.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2mmdtzhtb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2ypaulnbn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2vvgkfhqs.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ugneclrc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xofwmbcm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2zmvufnsp.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2uhmcpazb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vnieedmr.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dhyzwfao.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zwrtflmb.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pnzzjykb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2whlntulm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2nmvwifvh.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2xrtkfjwb.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2skmpvlme.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2saknpyfc.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2htaishkl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2irbhkljr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ookguric.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2dyoorybf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wyucuger.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2lfduzqdd.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2urjixdxf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2qjqqwpuj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2szpoesel.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2xrtrsgkt.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ivhukwqv.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gtvspbot.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2faclbhvr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hyccojhj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2cpfbznzl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cpgabovr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ercfwinr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sjnnryvz.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2fuulaytl.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2uwwlxuuj.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vzfjzdmc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2pmysofkq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2awykdawm.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jasukyar.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2guwyxoil.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ajtqcvdb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uxkirnyn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2inbrlwol.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fbbkkmkx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2irsojocu.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2npddzsmu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2srhhqkbw.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2eiwoutnf.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nsqieqrm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2fxjeywzo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wlsjhmrq.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bafydzha.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2baavyezd.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ejetyhtx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mhnfpsbs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2iblvlxch.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uhvkulus.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wsxtmrqp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sxxrrlby.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jzdursit.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qwxfmmwv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ytzgculg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tgxwsflv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2alyhjsqm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mjrxacsb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2kyrxaosg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2adslsxbn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2shclnngv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2zdqnczgs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2tpclclup.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nyzvgpim.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zpkllasl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2pemwjubq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2lqdedvae.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nenvevam.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2evlnnwqr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2fqctyflh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2rjktbcpg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kusifxui.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2iaddcozw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2tfoxqrnw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2mhkpmxkv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2amxusnvh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zkeiyiku.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2aqojweap.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2lvhhkkgq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2rvafzbwm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2yewfzvib.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2coohdqlz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iwjrsatw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2bcwuzmdm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2mcddxhne.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vuyvldki.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2reuhtdhs.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2jxxfrilq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ddjkmhok.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wzxekppy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sgzbhcxt.html


<!-- 参考信息 -->