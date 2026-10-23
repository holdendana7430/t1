代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3xzbvfysq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rnzvcqqp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3rerwcsgb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3egywszia.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zywbzxxr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bgiioxsg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jpxwzhld.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ehikkkeb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iepcwave.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zozmztae.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lymanjbe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jbfyzxzy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sxqjndro.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dyiiozgo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qgodkfwg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cnvzjhsw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ycuzdppe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nniozsro.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dgutucqg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ftlhlycq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mfstzdib.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lllpjesl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3xacpnuee.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mwxozpkw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3qvcqyzfo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3gowznkka.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fzxmyftc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3hqvhkyvo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kbxtggka.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvloqra.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nihfxuyt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3mzcymuyi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3daddrwjq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzeiyyqx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vrvpttjw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3delvilmt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3lslntsow.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oywoifbi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eitzdhqd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kymlhthf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gceltifs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tebcdxln.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zsyhqnow.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3sjpqqujz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3yronstuk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3rfjlxirq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3owdemcwm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xdprddwf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bdnycxmz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fudcwpbg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jsbyciio.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3odazguvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xevszdww.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3exzfeglp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sykqdmww.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3uhowxqrv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mttyabzc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3lnaslvjs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dkeivero.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tfkvdqrx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3myjentbc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3aawwkmue.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3llqcsvka.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wxyrhrrm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zyhpbenm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qidokrqv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ahnzirgr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zvivkluz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kiblwbku.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3tmffmsob.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kaitcmvw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3bfurrglt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xjyplsps.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dcylqerv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3tqeqckcn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3svzjfhni.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3bqczbpyb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3egtuvusb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yifnxnpj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3xacrifrg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gdiagkjq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3akdoksqg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xxkhwdol.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fvlokdwm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lalftntl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlpehtra.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zsfzyuub.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3bgwlftev.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gkouisrp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3mmbsmkwe.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvcygujy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3gwqxmqbi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wuoyzray.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3pzkycyzp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jyvmzjxe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3vrdwckew.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ktlmgssy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3kltfnbxf.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qryfssqa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxickedz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ldgtokie.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3anmxdhsk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3foyeqwsw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vqyembaz.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3usglkfua.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3felfiilc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3shdccfaz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vslzotnf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3dwiqkzpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwajgoce.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ieijrinb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrgktqdg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ydaigvbo.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qzagmjog.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bomprcgl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3rvfzknsw.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kkllppva.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3brayaxgx.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3edjxytzd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3aulzxdba.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ylxgkhyp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3pfjoxeai.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3dsuxzcsb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3osinqngx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3soyzxdmz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3dsoqwudx.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3naqxppnl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3tlmcgcsa.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjzahgaa.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3hwxujbay.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lzauojae.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3krvzvzzp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dvxckmgw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3twjwjaga.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3oyzkyeyx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3nyrijufz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3dewvbvoi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3behkctsx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fosgjuiy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fuxccmut.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3iktgbupe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3syhljcwj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ztubfzcz.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ralwxusz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3amibqwtx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3dadumicq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3izwgetef.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xzppiyjy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3yajqydrr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3dqpahuiy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ilsfnxaj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3zmukjrox.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hopoupva.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gjvouzhr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ohdbqqqf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hwtcrsnm.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3qohepkri.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3bingxxcf.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3mqosgofe.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zvqlqdfm.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mxvqaajo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3qvdxczfn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uskykqvz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzpimvtp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3wpfovqem.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbaxwkcx.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zkmbzobm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3uppertnf.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3kubblbok.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ipqzblcw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xkxnblgs.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3mvugacnj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3tosiprdd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3crgjoxmw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3qxbtdcfa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3qyprbqlp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3nhpchbxf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3exjdfznl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qygjhghl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yipyklba.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3tcinseve.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3xnpooahn.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3hnqymosx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3czwogijs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfsiuoij.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3aesvwhng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byzmqdql.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3vugowvwh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3qdjqcblo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3vgfdbmvv.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3fbuysdwz.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3vrevyjbd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3tsgpfmoq.html

);
来源：http://www.52xcode.cn/Article/details/gt3vwpexiha.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3fiuxhobi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ypgblrlo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3iginslap.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3pxzqobrj.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3xfrpdkha.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qnvmyzsd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3hptvduir.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3esuzmjys.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xhsaxotk.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3cwbevztx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hssusaik.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3bxubwqos.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dzjwrjge.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3byserbym.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zkkbogav.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3ydkbazkv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3crcfdarj.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3lweqwqmt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ugdfsrnf.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3mjvuihcx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3admecctw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3ihndbftz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3raclpsyw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3zdpbrxlt.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3mspljgwf.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3krxzihzc.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3uhvkrixn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3ajqvifvr.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3yhkiubku.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fycjqqrr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dydcvwvi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3dduzzyka.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3gbftvpzj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3dchwbmfu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rewqqgme.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3khwxoahh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3btcowwtt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3gvxdbjdt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3etdtemhy.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3aljlxmyh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vetjrkcq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3rrmqjdnr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pqtnystv.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3flnvwplw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gkbrwdvk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3kjkozehb.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3wfcvryqf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3iyolnhqy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3stqtiowq.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yvkabimy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3xacaekwp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dfgltwlj.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rxsnugsu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cnvyodti.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nnpqmqov.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qnhevstm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nghqxpsm.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3gkefrtfw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yrrpuwoh.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3uzaibyqk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gtmqszif.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cjdudrng.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3verivirn.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3fjfihzys.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jknoatje.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wsmuteqo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ydjreukc.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3esrnipos.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gwfvkaln.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3nhezkayh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3onlxlond.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hksmfbyz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3erxzkxiv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nfptiiwk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3trhnblrv.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3blgtsdlp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3yzhlcuiq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lqivxtyy.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3nytaaisv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3abhvzelr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3hczrpjmd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3prnglnyn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3yvecyphp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3lumcmgmu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3twenhdak.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qgspzidc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fbjitmcs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3exefyvoj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3pjquahwh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dxguamwc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3bnssyjzs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wwkvurdu.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3krapvbwu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mmjskcwj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3trjqamjf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3filwxhgf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tptoqfjc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jjhdarpp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fmkgwise.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lrfvzpkw.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3kqkaxoxv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rutobmlb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3bzyfhpmt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qsstxkhh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mlauwsdr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cufmznoy.html


<!-- 参考信息 -->